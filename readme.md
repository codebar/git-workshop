# Git Workshop for 24 Pull Requests

###Repository

The purpose of Git is to manage a project, or a set of files, as they change over time. Git stores this information in a data structure called a repository, commonly shortened to repo.

###Forking

Forking a repo allows you to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

Go onto the [codebar blog](https://github.com/codebar/blog) and fork the repo (top right of the webpage). This will create a copy of the repo on your own Github account, at github.com/[YourUserName]/blog.

Once this is done, you'll need to clone your forked repo into a folder on your machine so you can work on it:

```
$ git clone https://github.com/[YourUserName]/blog.git
```

Once this is cloned onto your machine you will need to open the `blog` folder and pull the **24PR-workshop-post** branch. To do this:

```
$ git checkout -b 24PR-workshop-post origin/24PR-workshop-post
```

This pulls down a branch that is currently not merged into master.

##Creating a new branch

You will now need to create your own banch that you can change some code on.

```
$ git checkout -b [new-branch-name]
```

This branch is where all your code amends will live untill merged in.

### Adding/Committing and pushing

For this tutorial there is a file `source/posts/2015-12-04-24-pull-requests.markdown`, please add your name and a little paragraph about your coding experience to date.

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

Navigate to the page of the repository, in this case the original [codebar blog page](https://github.com/codebar/blog). You should see a green prompt at the top of the page asking you to 'compare and pull request', click that prompt. You will then be navigated to a page that will ask you to describe what you did in the pull request, and the original branch that you are comparing against. Complete all of these required fields and click 'create pull request'. 

###Congratulations you have just done your first pull request :) 

#### You may want to refer to this [file](https://github.com/KimberleyCook/git-commands) for more git commands throughout the day. 
