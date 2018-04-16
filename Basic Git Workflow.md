# Git 

Git is a software that allows you to keep track of changes made to a project over time. Git works by recording the changes you make to a project, storing those changes, then allowing you to reference them as needed.

## 1. Initialize Git:
  We do this with:
  
    git init

The word init means initialize. The command sets up all the tools Git needs to begin tracking changes made to the project.

## 2. Git Workflow

Nice! We have a Git project. A Git project can be thought of as having three parts:

A Working Directory: where you'll be doing all the work: creating, editing, deleting and organizing files

A Staging Area: where you'll list changes you make to the working directory

A Repository: where Git permanently stores those changes as different versions of the project
![enter image description here](https://s19.postimg.cc/diswg6237/Git_Workflow.png)

The Git workflow consists of editing files in the working directory, adding files to the staging area, and saving changes to a Git repository. In Git, we save changes with a commit, which we will learn more about in this lesson. 

## 3. Check Git status
  
    git status


## 4. git add
In order for Git to start tracking file scene-1.txt , the file needs to be added to the staging area.
We can add a file to the staging area with:

    git add filename
    ex - git add scene-1.txt
   The word filename here refers to the name of the file you are editing, such as scene-1.txt.
## 5. git diff

 Imagine that we type another line in scene-1.txt. Since the file is tracked, we can check the differences between the working directory and the staging area with:
   
    
        git diff filename
    
    ex- git diff scene-1.txt


## 6. git commit

A commit is the last step in our Git workflow. A commit permanently stores changes from the staging area inside the repository.

git commit is the command we'll do next. However, one more bit of code is needed for a commit: the option -m followed by a message. Here's an example:

        git commit -m "Message"
    
Standard Conventions for Commit Messages:

- Must be in quotation marks
- Written in the present tense
- Should be brief (50 characters or less) when using -m    


## 7. git log

Often with Git, you'll need to refer back to an earlier version of a project. Commits are stored chronologically in the repository and can be viewed with:

    git log

In the output, notice:

A 40-character code, called a SHA, that uniquely identifies the commit. This appears in orange text.
>The commit author (you!)
The date and time of the commit
The commit message

## 8. Generalisations


You have now been introduced to the fundamental Git workflow. You learned a lot! Let's take a moment to generalize:

Git is the industry-standard version control system for web developers
Use Git commands to help keep track of changes made to a project:

 - git init creates a new Git repository 
 - git status inspects the contents of the working directory and staging area 
 - git add adds files from the working directory to the staging area
 - git diff shows the difference between the working directory and the staging area
 - git commit permanently stores file changes from the staging area in the repository
 - git log shows a list of all previous commits
 entities. 
