# Assignments & Solutions

## Assignment Submissions

**The below procedure should be completed once per week.** However, twice per cohort DSRs will run through **ALL** previous assignment submissions. (Feel free to split the load between both DSRs)
- First, one/two weeks before solo week
    - PL will send individual lists to students based on their completion statuses to catch up during solo week
- Second, the Tuesday after solo week

### Access Assignment Submissions in LEARN
1. **UNIT PROGRESS** tab
2. **<block_name>** use down arrow
3. <Assignment_name> use down arrow   
4. <Assignment_Submission> small circle indicates 'submitted'

### Update Assignment Status in HUB
1. Access your cohort's [main HUB](/RPP-DSR-Reference#quick-links) and choose the "Assignment Submissions" tab.
2. Look at the last SIX Learn assignments submissions that have passed their due date (This should equal out to about 3 weeks back) and update the spreadsheet with "Submitted" or "Not submitted."
	 - Example: Today is 6/22. Flask & Text Classification assignments are due today. I will look at the submissions for those and the 4 previous assignments (clustering, LDA, Image Processing, and CNNs) and update the spreadsheet.
3. Check that the due dates for the assignments are correct on Row 2. Please rearrange if the order of assignment sue dates are incorrect.
4. Update the B1 red cell with your initials, date, and time you've checked the assignments

## Incomplete Assignments

If a student has not submitted an assignment please complete ONE of the following:
1. Message the student and the PL asking why the student has not turned in an assignment. Use the following message:
    > - “Hi NAME! I hope you are doing well. I was checking assignment submissions and I saw that you have not turned in NAME OF ASSIGNMENT. Did you forget to submit the assignment in LEARN, or are you needing more time to work on this?”
    > - If the student needs more time, give them to next class to complete and leave a note in the submissions tab as a comment so the PL or next DSR will know that you've spoken to them about the submission
### **OR**
2. Contact the PL to reach out

<br />

> [* checking and updating assignment submissions how-to video](https://drive.google.com/file/d/1BvwxMJU055kYyfC1eC52urwPriOdBGa9/view?usp=sharing)

## Assignment Due Dates:
- In general, the due date is a week from the corresponding lecture.  
- Async assignments are due a week from that week's Saturday lecture.
- Paired assignments should be italicized

> [* updating due dates how-to video](https://drive.google.com/file/d/16eXyF5IjBbbd8CxRdG5m22Qt7EvyXzwe/view?usp=sharing)

## How to open the LEARN Modules for Upcoming Week
1. **SET UP** tab
2. **Content** tab
3. **<block_name>** block
4. click grey eyeball to right of <block_name>  
> Note: In an open block, the eyeball will disappear, but hovering over the <block_name> will reveal a green eyeball that can be clicked on to close the block.

> [* open learn modules for upcoming week how-to video](https://drive.google.com/file/d/16Stfq6gfBHQslPfDbP9OzCEp8A8c6BRr/view?usp=sharing)


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
