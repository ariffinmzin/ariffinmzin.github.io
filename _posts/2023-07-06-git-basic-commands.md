---
title: "Git Basic Commands"
author: ariffin
date: 2023-07-06 22:42:00 +0800
categories: [Blogging, Git and GitHub]
tags: [git and github]
---

# Unleashing the Power of Git: Your Guide to Mastering Basic Commands

Hey there! If you're into the world of programming, web development, or software engineering, you're probably no stranger to the fact that version control is your BFF. And when it comes to version control, what better tool to have in your arsenal than Git?

Today, we'll guide you through a fun-filled journey exploring the basics of Git and how to navigate through the process of creating, editing, committing, reverting, pushing, and pulling your HTML file. So, whether you're a newbie or just need a refresher, grab a cup of your favorite brew, and let's get this party started!

## Step 1: Initializing a Git Repository

First things first, you'll need to have Git installed on your system. Head over to [Git's official website](https://git-scm.com/downloads) and follow the installation guide suitable for your operating system.

Once you've done that, open your terminal or command prompt and navigate to the directory where you want your project to live. Then type the following command to initialize a new Git repository.

```bash
git init
```

And Voila! You've got yourself a new Git repository.

## Step 2: Creating an HTML File
For the purpose of our example, let's create a simple HTML file named `index.html`. Open your favorite text editor (Sublime Text, VS Code, you name it), and jot down some simple HTML like this:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First HTML File</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

Save the file in the same directory where you initialized your Git repository.

## Step 3: Adding and Committing the HTML File
Now that we have our HTML file, it's time to stage and commit it to our Git repository. Staging is like adding items to your shopping cart, and committing is like checking out at the register. Here's how we do it:

```bash
git add index.html
git commit -m "Initial commit - Add index.html"
```

The `add` command stages the file and the `commit` command saves it to the repository with a message describing what changes you made. Remember to keep these messages clear and informative, your future self will thank you!

## Step 4: Editing the HTML File and Making More Commits
Making changes is part of the development process. Let's say we want to add a paragraph to our HTML file. We edit our `index.html` to look like this:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First HTML File</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is my first HTML file on Git!</p>
</body>
</html>
```

We then stage and commit this change:

```bash
git add index.html
git commit -m "Add a paragraph to index.html"
```

## Step 5: Reverting Changes
Made a boo-boo and need to go back to a previous version of your file? Git's got your back with the `revert` command. Let's say we didn't actually want to add that paragraph. No problemo!

```bash
git log
```

This command will show you all the commits you've made. Each commit has a unique ID (called a SHA) at the top. Copy the SHA of the commit you want to revert, and then:

```bash
git revert <PASTE_COMMIT_SHA_HERE>
```

And just like that, Git will create a new commit that undoes the changes made in the specified commit. Remember to replace `<PASTE_COMMIT_SHA_HERE>` with the actual SHA of your commit. It will open a text editor for you to enter a commit message. You can use the default one provided by Git, or write a new one that explains why you are undoing the previous changes.

## Step 6: Pushing to a Remote Repository
So, you've made some rad changes, and now you want to share it with the world or maybe just a coworker. Time to push your local commits to a remote repository, like one hosted on GitHub. Let's create a new repository on GitHub (you'll need a GitHub account for this, of course).

Once you've created a new repository on GitHub, link it with your local repository and push your changes using these commands:

```bash
git remote add origin <PASTE_YOUR_REPO_URL_HERE>
git push -u origin master
```

Be sure to replace `<PASTE_YOUR_REPO_URL_HERE>` with your GitHub repository URL. The `remote add` command tells Git where your remote repository is hosted, and the `push` command sends your committed changes to this remote repository.

## Step 7: Pulling from a Remote Repository
If you're working with others, you'll need to keep your local repository updated with the changes they push to the remote repository. That's where the `pull` command comes into play:

```bash
git pull origin master
```

This will fetch all the new changes from the remote repository and merge them with your local repository.

And there you have it! With these Git basics under your belt, you're well on your way to becoming a Git whizz. Remember, coding is a journey, and every journey begins with a single step (or, in our case, a single `commit`). Happy coding!