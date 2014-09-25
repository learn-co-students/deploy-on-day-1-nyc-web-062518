---
  tags: deploy, team, git, pull request
  languages: html, css
  resources:
---

# Deploy on Day One

## History

Welcome to Flatiron! Every semester, a student index page is created. It looks something like [this](http://students.flatironschool.com/). Links from this page go to individual profiles, which look like [this](http://students.flatironschool.com/students/lauraconwill.html).

## Assignment

Your assignment is to create a student profile for someone sitting at your table. By the end of this project, every student should have a profile for themselves that was created by someone else and every student should have created a profile for someone else. If you're sitting at a table of four, it might be easiest to pair up. If you're sitting at a table of three, it might be easiest to create the profile of the student clockwise to you. If you're sitting at a...well you get the picture.

Now if you're anything like me, you might be freaking out and wondering, "Am I making a webapp?!?!" The answer is no. You're just working with HTML and file structures. You don't need to know Rails, JavaScript, or even Ruby for this project. No need to freak out. Calm down! Seriously, you're making the rest of us nervous!!!

## Structure

The structure of this project looks something like this:

```text
├── README.md
├── css
│   ├── css style sheets
│   └── fonts
│       └── font files
├── img
│   ├── lots of images here
│   ├── stripe_bg.gif
│   └── students
│       ├── student_name_background.jpg
│       ├── student_name_index.jpg
│       └── student_name_profile.jpg
├── index.html
├── js
│   └── javascipt files
└── students
    └── student_name.html
```

### Files you will need to alter:
* The only file you'll alter is `index.html`. 

### Files you will need to add:
* Add three pictures to the `img/students` folder (they can be jpg or png files):
  * A background picture
  * A picture for the index page
  * A picture for the profile page
* Add one HTML file to the `students/` folder. Use the `student_name.html` for reference. In fact, feel free to copy as much of the HTML from `student_name.html` into the new file you've created.

## Getting Started

### Group Logistics
* Figure out who is going to write whose profile.

![fork](/img/fork.png)
* Have one person at your table [fork](https://help.github.com/articles/fork-a-repo) this repo. This person should then send the link to their fork to everyone sitting at their table. 

![clone](/img/clone.png)
* Everyone at the table should then [clone](http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository) this forked repo.

### Individual Instructions

* Now that you have the repo, you'll want to get into it. 
  * Remember [cd](http://linux.about.com/od/commands/a/Example-Uses-Of-The-Command-Cd.htm)? When you type `pwd` into your terminal and the last part of the text that gets returned is `deploy-on-day-1...` you're in the right place.
  * ***NOTE In all the hypothetical examples, we're writing a profile for Zoe Perez.***

* Take a look at `index.html` and `students/student_name.html` in the browser.
  * You can do this many ways but one is by opening finder and right clicking on index.html, for example. Then click on "Open with" then the name of your favorite browser.

* From the root directory, [checkout a new branch](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging#Basic-Branching). This new branch's name should be the name of the student whose profile you're going to create.  
  * For instance, the branch would be titled `zoe-perez`.

* If you haven't already, switch to the branch you created. To make sure you're where you need to be, type `git branch` in your terminal. It should return the name of your assigned student emphazised with an asterisk and master.
  * For instance, typing `pwd` in the terminal would return:

```text
  master
* zoe-perez
```

* In this new branch, make a new HTML file in the `students/` folder. The file name should be the name of the student you're creating the profile for. Use the file `student_name.html` to see an example of what a profile's HTML could look like.
  * For instance, we would create a file `zoe_perez.html` in the main `students` folder.

* Still in this branch you created, add the three photos detailed above to the `img/students` folder. The student you're writing the profile for may have to email you their desired pictures or send you links to them, etc.
  * For instance, we would add a the pictures titled `zoe_perez_background.jpg`, `zoe_perez_index.jpg`, and `zoe_perez_profile.jpg` to the `students` folder that is inside the `img` folder.

* Once you've completed the profile, open up `index.html`. Use the prexisting template as a model and add a section for your fellow student.

* Once you're happy with the profile you've created and the changes you've made to the index page, type [git status](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Checking-the-Status-of-Your-Files). The the file you've altered, index.html, should appear in the "Tracked Files" section and the files you've created should appear in the "Untracked Files" section. 

* You'll want to [add](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Staging-Modified-Files) then [commit](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes) these changes with a message.

* Once you have added and commited properly, when you type `git status`, you should see "nothing to commit, working directory clean"


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
  - `cd 004.students.flatironschool.com`
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
