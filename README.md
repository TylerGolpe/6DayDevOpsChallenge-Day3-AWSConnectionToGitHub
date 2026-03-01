<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Connect a GitHub Repo with AWS

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-devops-github)

**Author:** Tyler Golpe  
**Email:** tylerogolpe@gmail.com

---

## Connect a GitHub Repo with AWS

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_dd9d254e)

---

## Introducing Today's Project!

In this project, I will be linking my AWS account to Github using access tokens.

### Key tools and concepts

Services I used were EC2, Git, and GitHub. All of these are standard for developers.

### Project reflection

This project took me approximately 30 minutes.

I continued this project today as I knew it wouldn't take very long, and I had already finished the previous "day" earlier in the morning, so I wanted to just continue with the boring stuff. 

This project is part two of a series of DevOps projects where I'm building a CI/CD pipeline! I'll be working on the next project either tonight or tomorrow. 

---

## Git and GitHub

Git is a tool for keeping track of changes to a code repository. It can be installed using your distribution's package manager and specifying "git"

GitHub is the host that stores your code repository's changes after pushing with Git. AWS also has their own version, but GitHub is more widely used.

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_efaadbf7)

---

## My local repository

A Git repository is a destination for your code and other project files to live for tracking and collaborating.

Git init will initialize your current folder as a repository. This repository is the "base" of what will be tracked & added to GitHub.

A branch in Git is a separate segment of the same project. Typically, the main/master branch is the live version of the project, while other brances are used for testing. Then, once a change is seen as bug-free, a pull-request will be made, requesting that branch's changes to be added to the main branch.

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_7bf21bae)

---

## To push local changes to GitHub, I ran three commands

### git add

The first command creates the "staging area" where all changes will be tracked. It says "Hey, all the files here I need to be uploaded" and gets them ready to be sent.

### git commit

The next command "commits" your changes with a message. Every commit should have a meaningful message. In this case, I simply used "Initial commit" since the project repository was still blank.

### git push

The third command will "push" the changes to our GitHub repository, and set the "main" branch as our priority when pushing from our local repo.

---

## Authentication

When I commit changes to GitHub, Git asks for my credentials because it needs to verify who I am. This is useful for project owners, as they don't have to think twice about where a commit is coming from, it's all tracked and supporting non-repudiation.

### Local Git identity

Git needs my name and email because it needs to log who I am definitively. 

Running git log showed me the log of git actions for the repository.

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_9a27ee3b)

---

## GitHub tokens

GitHub authentication failed when I entered my password because it is no longer supported for Git operations. We have to create an access token for our EC2 instance to push the files instead.

A GitHub token is a secure way of authenticating an application's programmatic access without entering the typical "root user" credentials. 

I set up a GitHub token by heading to my account settings and selecting the options to create a classic token. 

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_fa11169d)

---

## Making changes again

I wanted to see Git working in action, so I changed the lines in my index.jsp file of my webapp's main directory before pushing the changes and refreshing my browser.

The changes were displayed after the typical Git cycle of add, commit, push.

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_6becb2bc)

---

## Setting up a READMe file

A README file is the main explanatory or demonstratory file that should be in every GitHub repo. It's the best way of communicating your project's intentions and use-case to the world.

My README is written in Markdown because special characters are supported and can help you format text.

The default README file provided by the project includes a few basic sections that go over the "meat and potatoes" of the project. 

![Image](http://learn.nextwork.org/surprised_silver_peaceful_unicorn/uploads/aws-devops-github_c94976902)

---

---
