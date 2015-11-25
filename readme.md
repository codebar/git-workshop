# Git Workshop for 24 Pull Requests

###Repository

The purpose of Git is to manage a project, or a set of files, as they change over time. Git stores this information in a data structure called a repository, commonly shortened to repo.

###Forking

Forking a repo allows you to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

Go onto the [codebar blog](https://github.com/codebar/blog) and fork the repo into a folder on your machine.

##Creating a new branch

Once you have the repo on your machine you will want to create a new branch to change some code.

```
$ git checkout -b [new-branch-name]

```

This branch is where all your code amends will live untill merged in.

### Adding/Committing and pushing

For this tutorial there is a file in source/posts/[file to change], please add your name and a little paragraph about your coding experience to date.

In order for your changed code to be visible to the original developer you will need to add your changes to your local repo, commit them to the local repo then push them to the remote(original) repo. 

```
$ git add [file-name-you-changed]

$ git commit -m 'Here you can put a message of the changes you made'

$ git push -u origin [branch-name]

```
 If you have made multiple file amends you may want to do the following to add many files:

```
$ git add .
 
```

### Creating the pull request

Now that your code is pushed to origin you can do the pull request.

Navigate to the page of the repository, ,n this case the original [codebar blog page](https://github.com/codebar/blog). You should see a prompt telling you to do a pull request, click that prompt. You will be navigated to a page that will ask you to describe what you did in the pull request, and the orinal branch that you are comparing against. Complete all required fields and click submit. 

###Congrats you have just done your first pull request :)
