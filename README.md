# How to Git

## Installation ([Detailed information](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-14-04))

### Linux -
#### On a debian based distro -

`sudo apt-get update`

`sudo apt-get install git`
#### On Fedora -

`sudo yum install git`

#### On several other Unix flavours - 

[https://git-scm.com/download/linux](https://git-scm.com/download/linux)

### Windows(7 or later) - https://github.com/git-for-windows/git/releases/

### Configure :

`git config --global user.name "Your Name"`

`git config --global user.email "youremail@domain.com"`

`git config --list`

## Let's get started!

### Two ways to start - 

1. [Create your own project](#1-creating-a-project)
2. [Contribute to a project](#2-contributing-to-a-project)

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

#### Git it 

`git status` (use whenever in doubt about the status of the files)

`git add <file>` (track the files)

`git commit -m "some relevant message"` (commit the files)

`git push origin master` (Push master branch to origin)

**Add.Commit.Push.**

These are the three git commands that will be used **heavily**. Keep them handy!

#### Create branches 

`git branch` (List out the available branches)

`git branch <branch_name>` (Why do we need branches? What happens after branching?) 

`git checkout <branch_name>` (Switch branches)

After 'gitting it'.. 

#### Merge the branches  

1. Github (Compare and Pull Request) 
2. Command line -
After committing
`git checkout master`
																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																																		
`git merge <branch_name>`

And then push master to origin.

What is **gitignore** and why is it important?

#### Resolving Conflicts

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

**Add.Commit.Push.**

Create a pull request.

Wait.Review.Push.Enjoy!

## How to rebase?

[Reference link](https://github.com/edx/edx-platform/wiki/How-to-Rebase-a-Pull-Request)
### What you've done till now
```
git clone https://github.com/my-username/how-to-git.git
cd how-to-git
git checkout -b my-branch
```

### Add the official repo as a remote

`git remote add howtogit https://github.com/nirajpandkar/how-to-git.git`

###Check the new added remote 
`git remote -v`

###Fetch the latest version of master
`git fetch howtogit`

#### Squash changes
#### Reword commits

### Perform the rebase finally

git rebase howtogit/master

You may get conflicts. 
After resolving those conflicts **Add.Commit.**

Wait.. No **Push.**?
Yes. Here you first `git rebase --continue`
And then `git push -f origin master`

Your pull request will be updated!! Successfully rebased!

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

rebase

## Reference Links

#### Understanding Git(in depth) - 
[Git Parable](http://tom.preston-werner.com/2009/05/19/the-git-parable.html)

#### Git Glossary
[Glossary](https://www.kernel.org/pub/software/scm/git/docs/gitglossary.html)