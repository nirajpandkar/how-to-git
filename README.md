# How to Git

## Installation ([Detailed information](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-14-04))

### On Linux -

`sudo apt-get update`

`sudo apt-get install git`

### On Windows(7 or later) - https://desktop.github.com/

### Configure :

`git config --global user.name "Your Name"`

`git config --global user.email "youremail@domain.com"`

`git config --list`

## Let's get started!

### Two ways to start - 

1. [Create your own project](#1.creatnigaproject)
2. [Contribute to a project]()

#### 1. Creating a project

Initialize your repository on your local machine - 

`git init`

`git remote add origin <repo_url.git>`

or 

`git clone <repo_url.git>`

Create an html file (index.html) -
 
```
<html>
<head>
<title>
	First contribution!
</title>
</head>
<body>
	<h1> C-Cube </h1>
	<h2>Learn.Join.Compete.</h2>
</body>
</html>
```

Git it - (Untracked files)

`git status` (use whenever in doubt about the status of the files)

`git add <file>` (track the files)

`git commit -m "some relevant message"` (commit the files)

`git push origin master` (Push master branch to origin)

These are the four git commands that will be used **heavily**. Keep them handy!

Create branches - 

`git branch` (List out the available branches)
`git branch <branch_name>` (Why do we need branches? What happens after branching?) 
`git checkout <branch_name>` (Switch branches)

After 'gitting it' merge the branches - 

1. Github (Compare and Pull Request) 
2. Command line -
After committing
`git checkout master`
`git merge <branch_name>`

And then push master to origin.

What is **gitignore** and why is it important?

#### Commit Collision

```
<<<<<<< HEAD
Code that you have written
=======
Your friend's code
>>>>>>> 90e9cff27a42949307694d35d5ea5138e2d11a1a
```

#### 2. Contributing to a project
`git clone <repo_url.git>`

Make a new branch (good practice)

Make awesome changes

Add.Commit.Push.

Create a pull request.

Wait.Review.Push.Enjoy!


## **Terminologies:**

SVN

remote

local

origin

master

commit

track

branches

gitignore