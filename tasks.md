# Daily & Weekly Tasks 

## Every class day:
- Take attendance (*If the student is not in class, reach out to PL or the student directly)
- Remember to RECORD lectures
- Open LEARN modules, assessments, and assignments for the day
- Check and update cohort solutions repo
- Check to see if an assessment grading is needed - grade and message the PL when the HUB spreadsheet has been updated
- Check to make sure previous class recording has been uploaded to the cohort spreadsheet. [Instructions on linking the recording in Cohort Spreadheet Calendar](assignments_sols.md#Post-Lecture-Recording-In-Cohort-Spreadsheet-Calendar-After-it-Processes)
- Check assignments due today and check late submissions from the previous week. Update assignment submission HUB. If a student has not submitted an assignment please complete ONE of the following:
	- 1. Message the student and the PL asking why the student has not turned in an assignment. Use the following message:
		> - “Hi NAME! I hope you are doing well. I was checking assignment submissions and I saw that you have not turned in NAME OF ASSIGNMENT. Did you forget to submit the assignment in LEARN, or are you needing more time to work on this?”
		> - If the student needs more time, give them to next class to complete and leave a note in the submissions tab as a comment so the PL or next DSR will know that you've spoken to them about the submission
	### **OR**
	- 2. Contact the PL to reach out

- *Check "non-lecture day" links below for additional instructions

- **Send a slack message out at the end of class on assignments (including async), assessments, and Capstone proposal due dates coming up the following week (include dates)
	- bold async assignment(s)
	- italicize paired assignment(s)

## Weekly Tasks:
> Done Saturdays and [Career Services](#Career-Services-Days) Days
- [Assign pair programming](pair_programming.md) groups and assign a “scheduler” 2 weeks out 
- Check to see if your [office hours](calendars.md#DSR-Coverage-Calendars) are correct for the following 2 weeks
- Open the needed LEARN modules for the upcoming week
- Check next week’s schedule ([spreadsheet](https://docs.google.com/spreadsheets/d/1L5IDfOIK6u2oWkt0Io-SYhtJlluVLCJbnWn0E-N_pqs/edit#gid=0) & [google calendar](calendars.md#Cohort-Google-Calendars)) following items for accuracy:
	- (spreadsheet calendar should be most up to date)
	- Check lecture, retro, assessment, case-study, capstones, break dates
	- Check that all recordings have been uploaded to spreadsheet (update if they have not been uploaded)

	[Lecture Days](#Lecture-Days)  

	[Assessment Days](#Assessment-Days) 

	[Case Study Days](#Case-Study-Days)  

	[Capstone Days](#Capstone-Days) 

	[Retro Days](#Retro-Days)
	
	[Career Services Days](#Career-Services-Days)  

______________

# Lecture Days

## Record Lecture
> All the sticky notes & alarms in the world aren't as effective as multiple people checking that the lectures is being recorded. Let the cohort know you appreciate their help.

## Provide Access to Assignment Repo

> Open at the beginning of class, **not prior to lecture**
1. Settings
2. Manage Access
3. Enter and Confirm your password
4. Invite teams or people (READ Access)
5. *For RPP2, add **GalvanizeDataScience/21-02-ds-rpp**
6. *For RPP2, Confirm: Add GalvanizeDataScience/21-02-ds-rpp

> [* granting access to assignment repo how to video](https://drive.google.com/file/d/1UgR1OuQ_9dy9LSDXtgmXyxRhnAFqVEhH/view?usp=sharing)

### Add Solutions to Cohort's Solutions Repo

> [Galvanize Main Solutions Repo](https://github.com/GalvanizeDataScience/solutions)
> ^All the solution directories are here^

- [RPP2 Solutions Repo](https://github.com/GalvanizeDataScience/solutions-rpp2)
- [RPP3 Solutions Repo](https://github.com/GalvanizeDataScience/solutions-rpp2)
---

## RPP2 Example: 

**ONLY DO THIS PART THE FIRST TIME YOU ADD SOLUTIONS:**
```bash
git clone https://github.com/GalvanizeDataScience/solutions-rpp2.git
cd solutions-rpp2/  # Navigate to the directory you cloned to on your machine
git remote add solutions https://github.com/GalvanizeDataScience/solutions.git
git fetch solutions main
```

**DO THIS EVERY TIME YOU ADD SOLUTIONS:**
```bash
cd solutions-rpp2/  # Navigate to the directory you cloned to on your machine
git pull
git fetch solutions main
# > (using perceptrons as an example)
git checkout solutions/main perceptrons
git add .
git commit -m 'add perceptrons solutions'
git push
```

> [* add solutions to cohort's solutions repo how to video](https://drive.google.com/file/d/1-bMnSAy1uYL60b3aFw4e72U7_M1dByAN/view?usp=sharing)

## Post Lecture Recording In Cohort Spreadsheet Calendar After it Processes

Instructions for Listing Lecture recordings:
1. Locate recording in Zoom (Zoom login available in HUB: Important Docs tab)
2. Rename lecture recording
> - edit "RPT DSI staff's Personal Meeting Room" to reflect cohort number and lecture title (e.g. RPP3 Graph Searching Lecture)
> - edit "Recording 1" to same title (e.g. RPP3 Graph Searching Lecture)
> - If there are 2 recordings for the day, label the recordings separately
3. Link lecture recording in Cohort Spreadsheet Calendar

______________

# Assessment Days 

## Opening Assessment in LEARN 

> **TWO eyeballs to click!**

1. **SET UP**
2. **Content** tab
3. **Assessments** block
4. **DSI Assessment #** click first eyeball
5. click dropdown arrow to left of **DSI Assessment #**
6. click second eyeball

> [* opening assessments in Learn how to video](https://drive.google.com/file/d/1L_zHyMqH56RJAw6YmKtpJfbVEJH8JeJc/view?usp=sharing)

## Timing Assessment 
- 60 minute strict time limit
- Count down announcements at: 30, 15, 5 minutes left

## Checking Submission of Assessment 
1. **Go to Cohort LEARN page
2. **DSI Assesment_#** block 
3. **Results** table   
4. **Status** column

## Adding Assessment Solutions to the Solutions repo

```bash
cd Desktop/Galvanize/RPP2/solutions-rpp2 # navigate into solutions repo 
git pull
git fetch solutions main
git checkout solutions/main assessments/assessment-0 # using 0 as an example
git add .
git commit -m 'add assessment-0 solutions'
git push
```

[* add assessment solutions to cohort's solutions repo how to video](https://drive.google.com/file/d/1c5u2M1G9GcI6baEgayPEBUhRXYw9thLg/view?usp=sharing)


## Grading Assessments
- ### In LEARN  
> - You can find the cohort LEARN links at the top of this Repo or in the cohort hub

- ### In Hub (2 places to input grades)
1. You can find the cohort HUB links at the top of this Repo 
2. Then go to "Assessments" Tab
3. In the top left corner you will find a link to the Assessment Full Grading Tracking Doc 
4. Update the Full Grading Tracking Doc first and then in the assessments tab

[* grading assessments how to video]()

Assessment statistics will populate after inputs are complete, which can be used to add statistics to Learn:

### Adding Assessment Statistics & Solutions to Learn
[RPP2 Learn Assessment Solution Block](https://learn-2.galvanize.com/cohorts/2432/blocks/1045/content_files/01-assessment-solutions/01-solutions.md)

[* editing learn to add assessment statistics & solutions link how to video](https://drive.google.com/file/d/1dNWeRkPHVlmTwg8TEfPE3YWnp4Hytu1U/view?usp=sharing)

______________

# Case Study Days  
## Generate Groups of 3/4 students  
> Simple code for random list of RPP2 students, which can be used to choose pairs, groups of size k < n, and order of presentations: 

```python
import numpy as np
RPP2_students = ['Becky_MDT', 'Bahar_PST', 'Andrew_EST', 'Mekdi_PST', 'Tony_PST', 'Robert_CT',
			'Sean_PST?', 'Nick_PST', 'Reza_CT', 'Bobby_AZ', 'Di_PST', 'Gary_EST', 
			'Matthew_EST', 'Shaheer_AZ', 'Marwah_PST']

np.random.choice(RPP2_students, replace=False, size=len(RPP2_students))
```

## Assign breakout rooms 

## Progress checks

1. MVP plan

> - use MVP+, MVP++, future work to handle overly optimistic plans
> - plan should include hypothetic audience

2. Github repo  
> forked by student A  
> cloned from student A by other team members 

- [Ryan & Heather example video](https://zoom.us/rec/share/WYhK0DE1ZBs4lvN33JDCp3eMHl7QTycVjlaRXbWCgaXcVvwJ8CBzsrVFqjvMln1T.oETxz6XDF0QB1LuA?startTime=1616691949000)
> - suggest VSCode Live Share for README.md  

3. Slide deck/presentation tool started  

______________

# Capstone Days    

## Manually Assign breakout rooms 

## Stand-ups
> [RPP2 Stand-ups Sheet](https://docs.google.com/spreadsheets/d/1lztQRmiV1DQrzRyrgY0Lc_VqVFRYh7hXf0kuqDLs66k/edit#gid=0) 
Check:
1. Well defined MVP
2. Cohesive, narrow Story
3. GitHub repo + README + Slide Deck started

- Elevator Pitch (30 second engaging overview) 
- Follow-up on meeting goals from last stand-up
- Goals for today
- ABC always be committing

______________

# Career Services Days  

- ### Record with permission from CSM

- ### This is an appropriate time for DSRs to turn off camera and complete [other tasks](#Weekly-Tasks)

## Post CSM recording after it processes 
- edit recording name to include: *instructor, topic(s), date*
- check that no passcode is required
  
- ### Add zoom link in career services videos markdown file in VSCode:
	```bash
	cd dsi-learn-welcome-template
	git pull  
	git checkout RPP2 
	git pull  
	code .
	```

- ### Save changes:

	```bash
	learn preview -o .
	git add .
	git commit -m 'added CSM video'
	git push origin RPP2
	```

- ### In Learn:
	1. **SET UP** tab
	2. **Repos** tab
	3. **<block_name>** block will have a green 'updates' oval
	4. click sync arrows OR 3 vertical dots to right (choose update branch) of <block_name>  
	5. Double check that the changes are working in the student facing Learn block.

> [* add Zoom lecture recording to Learn how to video](https://drive.google.com/file/d/1HHMIrfLhJuhUm20fqOLfy-5EEF-cjxKJ/view?usp=sharing)
