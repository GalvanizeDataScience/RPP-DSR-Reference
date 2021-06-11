# Assignments & Solutions

## Assignment Submissions

### Checking Assignment Submissions in LEARN
1. **UNIT PROGRESS** tab
2. **<block_name>** use down arrow
3. <Assignment_name> use down arrow   
4. <Assignment_Submission> small circle indicates 'submitted'

### After checking submissions in LEARN, update Assignment Submission Sheet in HUB 

> A one-class grace has been the norm. For example, if the assignment is due on Tuesday, checking for that assignment submission + updating the google sheet on Thursday worked well. At the discretion of the instructor/PL, students may ask for an extension to the due date.

> [* checking and updating assignment submissions how to video](https://drive.google.com/file/d/1BvwxMJU055kYyfC1eC52urwPriOdBGa9/view?usp=sharing)

## Assignment Due Dates:
- In general, the due date is a week from the corresponding lecture.  
- Async assignments are due a week from that week's Saturday lecture.
- Paired assignments should be italicized

> [* updating due dates how to video](https://drive.google.com/file/d/16eXyF5IjBbbd8CxRdG5m22Qt7EvyXzwe/view?usp=sharing)

## How to open the LEARN Modules for Upcoming Week
1. **SET UP** tab
2. **Content** tab
3. **<block_name>** block
4. click grey eyeball to right of <block_name>  
> Note: In an open block, the eyeball will disappear, but hovering over the <block_name> will reveal a green eyeball that can be clicked on to close the block.

> [* open learn modules for upcoming week how to video](https://drive.google.com/file/d/16Stfq6gfBHQslPfDbP9OzCEp8A8c6BRr/view?usp=sharing)


> [GitHub gSchool](https://github.com/gSchool)  *(You can find the cohort LEARN links at the top of this Repo or in the cohort hub)

> [RPP2 Solutions Repo Link](https://github.com/GalvanizeDataScience/solutions-rpp2)

> [RPP3 Solutions Repo Link](https://github.com/GalvanizeDataScience/solutions-RPP3)


## JUST ONE TIME, get access to gSchool Learn

Follow the repo or the steps below

1. [Install Learn in terminal](https://github.com/gSchool/glearn-cli/blob/master/README.md)

```bash
brew tap gSchool/learn
brew install learn
brew list # look for 'learn'
learn set --api_token=<api token found in “API Token” tab under username in top right corner of Learn>
```
[Learn site API token generator](https://learn-2.galvanize.com/api_token)

> If you see this error:

> Error: The following directories are not writable by your user: /usr/local/bin. You should change the ownership of these directories to your user.
* use the suggestion the terminal gives
```bash
sudo chown -R $(whoami) /usr/local/bin
```
* use brew doctor to find any warnings you might have with brew

**Create a directory to store all the Learn repos: Desktop/Galvanize/RPP2/LEARN**

### For each Learn block, clone learn gSchool module into your Learn directory
> if you have already cloned the repo,
> - You don't need to re-clone the repo, just navigate in to repo
> - REMEMBER TO PULL after navigating into repo

```bash
cd Desktop/Galvanize/LEARN
git clone https://github.com/gSchool/dsi-learn-clustering-methods.git # if not yet cloned
cd dsi-learn-clustering-methods
git pull origin RPP2  # git pull will not update all branches
git checkout RPP2 
code .
```
Make necessary changes in VSCode markdown file(s)

Save changes

```bash
git status  # will  show the modified files
learn preview -o .  # opens a 'practice' Learn block to see repo after changes
git add .
git commit -m 'description of changes'
git push origin RPP2
```

In Learn:
1. **SET UP** tab
2. **Repos** tab
3. **<block_name>** block will have a green 'updates' oval
4. click sync arrows OR 3 vertical dots to right (choose update branch) of <block_name>  
5. Double check that the changes are working in the student facing Learn block.

[* editing Learn (fix solutions link example)](https://drive.google.com/file/d/1n-1kg-IupQXr9SPQNdlOMcEk-H0r0mGz/view?usp=sharing)


[Announcement Example Image](https://drive.google.com/file/d/1LzQ-3ANuL5Tuwv6pitsJpISPrPRVKRWg/view?usp=sharing)