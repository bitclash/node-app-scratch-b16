d# UXE - Node app from scratch

For this assignment, students will be required to build a UI module example view using Node and libsass with JavaScript(jQuery) and prepare for deployment to Heroku.



## Assignment description

Using what we have discussed for the past two days, the goal of this assignment is to build a Node/Express application from scratch, add libsass and build an example module using all the techniques learned to date for building elemental UIs.

An extension of this assignment is to build your own Bower package that is registered with Bower.io, you can distribute via Github and is 'imported' to your project.

### Things I am looking for:

* Using Express to build a new Node project
* Make appropriate use of
  * .gitignore
  * package.json
  * bower.json
  * readme.md files that explain install and set up instructions
* Install libsass using Grunt to process the Sass
* Using a modular Sass framework to build an example UI module
* Include some jQuery for effect
* Deploy to Heroku



## Submitting assignments

Submitting assignments for this course will require leveraging some of the more advanced features of Github. These features will not only improve your knowledge of Git and Github, but also provide practice exercises for working on a distributed project with a large team.

## How to submit an assignment

In order to submit assignments, please use the following steps

1. [Fork this repo][1] so that you have a working version
1. [Clone the forked repo][2] to your local computer
1. Create a folder named with your name, example `dale-sande`
1. Once completed with your assignment, commit code to the master branch and push to Github `git push origin master`
1. From __your fork__ of the project, initiate a pull request to the parent repo

## Assignment review

When a pull request is initiated, I will be notified of the update and comment on the submitted assignment via Github tools.

## Keeping your local repo up to date
Your local repo will be an independent version of the original repo from the moment you fork the repo. In order to keep your local repo up to date with the original repo, you need to do what is called an [upstream pull][3].

To manage an upstream pull, I suggest updating your `.bash_profile` and your `.gitconfig` file with easy to remember aliases.

### .bash_profile

In your `.bash_profile` add the following alias

```
alias upstream="git remote add upstream \$@"
```

From the command line you simply need to refer to the alias and add the path to the upstream repo as shown in the following example.

```
$ upstream https://github.com/blackfalcon/unicorn-class-css-section.git
```

Once the upstream repo is configured for your local repo, this never needs to be reset again, unless you delete your local repo.

### .gitconfig
In your `.gitconfig` add the following alias

```
[alias]
  pu = !"git fetch origin -v; git fetch upstream -v; git merge upstream/master"
```

From the command line, within the project repo, enter the following command to pull latest code from the upstream master.

```
git pu
```




[1]:https://help.github.com/articles/fork-a-repo
[2]:https://help.github.com/articles/fork-a-repo#step-2-clone-your-fork
[3]:https://help.github.com/articles/syncing-a-fork
