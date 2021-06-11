# Help Desk  
Encourage students to use the assignments channel to troubleshoot problems. Teach students to fish. The goal is helping the student find the answer, not providing the answer.

_______________

# Common-Fixes

## Docker  

> Ubuntu users may need to use sudo before docker commands
> https://stackoverflow.com/questions/48957195/how-to-fix-docker-got-permission-denied-issue


> If you do a git command with an open docker container, you may have to stop the container in order for the updates to show up.
> https://github.com/moby/moby/issues/15793#issuecomment-135411504


- ### sparkbook
> - $ docker run --name sparkbook -p 8881:8888 -v "$PWD":/home/jovyan/work jupyter/pyspark-notebook start.sh jupyter lab --LabApp.token=''

- ### pgserv  
> - $ docker run --name pgserv -d -p 5432:5432 -v "$PWD":/home/data -e POSTGRES_PASSWORD='galvanize' skylarenglish/galvanize:galv_db

> ^only do this once. If there is a problem:

		docker rm pgserv or docker container rm pgserv  and run again.
	docker start pgserv
	docker exec -it pgserv bash
	cd home/data/*from root of container 
	To leave the container:
	exit
	Docker stop pgserv
____

psycopg2 Install probs, try:
	
	conda update --all
	conda install psycopg2 
____

Working with psycopg2 in notebook/script?
	
	import psycopg2 as pg2
	conn = pg2.connect(dbname='readychef',
			     host='localhost',
			     user='postgres',
			     password='galvanize')
	cur = conn.cursor()
	query = '''select * from events limit 10;'''
	cur.execute(query)
	for row in cur:
	    print(row)


### mongoserver  

> If you get into the root directory and can’t navigate to home/data/…
(probably means the docker container ‘mongoserver’ wasn’t initially run with the right path)
From docker mongoserver root:

	```bash
	exit
	docker stop mongoserver
	docker rm mongoserver
	$ docker run --name mongoserver -p 27017:27017 -v "$PWD":/home/data -d mongo
	```

### tensorflow
    ```bash 
    docker run -it --name tensorflow -p 8888:8888 -v "$PWD":/tf tensorflow/tensorflow:2.0.0a0-py3-jupyter
     
    docker start tensorflow
    docker exec -it tensorflow bash
    ```
    Navigate to repo if you want 
    cd <path>
    In browser type: localhost:8888/
    To get token (if you don’t have a password set up)
    jupyter notebook list
    Something like this will allow you to copy and paste the highlighted part: token=f47d7c92d31140b3e12c0a68703c0a7e64944133a9e149e9
    Hopefully now, just navigate to the the repo/project
    To exit the container (all work show be saved on your local version too)
    exit
    ```bash
    docker stop tensorflow
    docker ps (to make sure)
    ```
## Github  

[Git Reference Doc](https://github.com/GalvanizeDataScience/course-outline/blob/21-02-DS-RPP/quick-reference/Git.pdf)


### [Kacie's Git Review](https://zoom.us/rec/share/woTbzJ12anB-q_dDd6_g5K_6k6ydmgxMzWVGLncsBQ7hnV_nVNwdfHxNnJuZbS2w.7pkatu8jYvAJ5477?startTime=1619659988000)

### Lecture Pulling
To clone just lectures from the RPT branch

	```bash
	git clone -b RPT --single-branch https://github.com/GalvanizeDataScience/lectures.git
	```

Tired of having to add your credentials to the terminal each time you want to clone or push?
	```bash
	git config --global credential.helper store
	git config --global credential.helper cache
	```
OR

	```bash
	git config --global credential.helper 'cache --timeout=3600'
	```

## Unix



## VSCode Environment
> For the unix assignment, when I try to put the 2015_goog_sorted.csv file into the plot_stock_prices.py code, VSCode and Pylint gives an import error for matplotlib. How do I fix this?
> answer:
> I figured out how to get this to work. I needed to set up the anaconda environment by typing conda activate env into my python console. The environment can be found by typing 
conda info --envs into the console.
____


## Mac
- “I've run into this problem whenever I update my macbook. “
> xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun  

> SOLN:

	```bash
	xcode-select --install
	```

## Linux/Unix

> TIME TROUBLE windows vs unix.
> Anyone irritated by the time in windows being off after using dual-boot UNIX?
this command (in unix) will tell unix to use local time and then windows and unix Times will play nice.

	```bash
	timedatectl set-local-rtc 1 --adjust-system-clock
	```

> If you're having trouble opening jupyter on a linux machine, it might be because you're using chrome, I've never had any problems with firefox. 

## Windows (even though the program may not 'technically' support windows)

> Okay I think the substitution for $PWD is %cd%. At least that’s what this article is telling me. https://stackoverflow.com/questions/35767929/using-docker-via-windows-console-includes-invalid-characters-pwd-for-a-local-v