---
  tags: deploy, team, git, pull request
  languages: html, css
---
#:confetti_ball: :bowtie: Welcome to The Flatiron School! :tada: :fireworks:

# Deploy on Day One!

### Skills: HTML, CSS, Git, deploying

## Instructions

Here is your first assignment! You're going to add yourself to the student section of [FlatironSchool.com](http://students.flatironschool.com) and create your own [profile](http://students.flatironschool.com/students/tiffany_peon_profile.html) page. 

You will be working in a team of 4 people.  At the end of the project, you'll have 4 new html files in the students directory one for each student.

## Deliverable:

1. yourprofile.html with a layout and content.
2. A git branch named `yourname-profile` along with a pull request to merge your branch into `master`. If you'd like to make things easier, you can also have a team branch `teamname-profiles` and just one pull request to merge that branch into `master`.

## FAQ

- Am I making a webapp?
  - NO
- Do I need rails?
  - NO
- Is there any reason I should be on Hacker News Today?
  - NO
- Do I need to change the index page?
  - The styles shouldn't change, the content of the HTML should

You can use the following link as a reference [students index](http://students.flatironschool.com/)

Check out different students profiles, be creative, and don't copy exactly.
Please read/skim this whole document before starting. Here's a few helpful tips...

- You'll have ~3hrs to complete this.
- If you feel stuck, ask for help.
- Don't get bogged down in git!
  - During this project we'd like you to become familiar with clone, pull, branch, checkout, and push but not all are required or expected.
  - **Keep in mind everyone in the class will be pushing to the same repository.**  Think about using a workflow with your teammates that will minimize conflicts.
- Many of you will want to know the right way to do it, but However your team decides they want to tackle things is the right way to do it.
- Types of questions you'll probably want to ask that we'd like you to decide with your group.
  - Should each member of the group have their own stylesheet or all share one?
  - Should we all work on one computer or each do our own and use git to manage merging our work together?
  - How do we put all our changes into one repository?
- The most important things are getting something working and learning to work as a team. There really are no wrong answers.
- Have fun with your new best friends!

## Steps

Note: Anywhere you see "yourname" please don't literally type this, please insert your actual name
- Clone the students website to your code directory.
  - `git clone git@github.com:flatiron-school-students/004.students.flatironschool.com.git`
- cd into the directory you just cloned
  - `cd 004.students.flatironschool.com.git`
- Create a feature branch for your profile
  - ```git checkout -b add-profile-yourname```
- Create your profile page within the students directory and name it yourname.html
  - ```touch students/yourname.html```
  - open the html in your favorite text editor and make your profile!
- Add it, commit, push
    - ```git add .```
    - ```git commit -m "Add profile for yourname"```
    - ```git push origin localbranchname```
    - To confirm this worked you can do ```git branch -a``` which will show the remote branch on github.com you just created when you pushed
    - Note: localbranchname should be add-profile-yourname

Create a pull request to merge your feature branch
  - Go to https://github.com/flatiron-school-students/004.students.flatironschool.com and click on the pull request button
  - This brings you to a screen where the left side is the place you're submitting the request to (flatironschool the master branch)
  - The right side of the screen is the branch and repo you are submitting from.  So you should select your branch which will take you to the pull request screen.  Fill in some details and submit the request.  Note you can @aviflombaum in the comment of your request to automatically let avi know you submitted the pull request.

## Profile requirements

Please collect the following content for your profiles. This content doesn't have to be finalized, but you need something. You'll be using this content as the project evolves for your resume and other profiles online, including the student site. If you have the data in an easy to use / read / copy text file, it makes putting it in different mediums easier.

- Your Name
- Github Username
- Blog Url (if you don't already have a blog it will be githubusername.github.io)
- Tagline
- Profile Picture (something normal, a headshot, of a good reusable size that can be easily cropped)
- Treehouse Account
- CoderWall Account
- CodeSchool Account
- Favorite Websites
- Previous Work Experience
- Short Bio
- Twitter URL
- LinkedIn URL
- Education

You can submit this via a GIST URL.

For example: https://gist.github.com/aviflombaum/015ee85d38e9009e012f

## Resources
Here are some Git workflow tutorials you can check out.  Don't get bogged down in Git!

- http://scottchacon.com/2011/08/31/github-flow.html

- https://github.com/diaspora/diaspora/wiki/Git-Workflow

- http://mettadore.com/analysis/a-simple-git-rebase-workflow-explained/

- http://zachholman.com/talk/how-github-uses-github-to-build-github

- https://openshift.redhat.com/community/wiki/github-workflow-for-submitting-pull-requests

## Issues

A common issue is not being able to authenticate with github. You need to use https/ssh correctly when cloning the repository in order to be authenticated with github. Checkout and follow:

- [setup git](https://help.github.com/articles/set-up-git)
- [https cloning errors](https://help.github.com/articles/https-cloning-errors)
- [setting up ssh](https://help.github.com/articles/generating-ssh-keys)

## A note about `master` branch

The `master` branch of a project is NEVER a place to do any work. `master` is considered the build and you never break the build. So make sure you are not working or committing to the `master` branch.

**We highly recommend getting ssh setup correctly**

### Good luck and have fun!
