---
title: "How to 'Git' ?"
seoTitle: "How to Git "
seoDescription: "Learn Git basics: installation, features, version control, commands, and examples. Start coding hands-on practice with examples, demo links & git resources."
datePublished: Mon Mar 25 2024 18:30:00 GMT+0000 (Coordinated Universal Time)
cuid: clvuabn0p00000ai1elujasq2
slug: how-to-git
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1714958762369/cd955d07-fa7d-4a79-872e-3c4a84db5b14.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1714958744928/1387d95a-7f7b-4f85-8908-ec9bffa6151d.png
tags: github, version-control, git, hashnode, gitlab, versioning, womenwhotech, gitcommands, git-github-version-control-linux-git-commands-github-repositories-cheat-sheet-git-branching-git-workflow-collaboration-git-history-git-commit-git-merge-git-rebase-git-pull-request-git-fork-git-stash-git-remote-git-ignore-git-hooks-github-issues-github-actions-github-pages-github-security-git-for-beginners-advanced-git-techniques-github-collaboration-git-integration-git-flow-git-best-practices, git-commands-for-beginners, installation-guide, git-with-examples, understanding-git, git-easy, khushitrivedi

---

This blog is specifically for the total newbies, who are either confused about the version control system, or have been a total beginner in tech.

<mark>NOTE: GIT and GITHUB are two different things! (Git isn't a part / subset of GitHub, or vice versa)</mark>

---

# [What is Git?](https://www.youtube.com/embed/nqCY3njHg2U?start=1075&end=1569)

Linus Torvalds, the developer who created Linux OS, created Git in 2008 with the intent to create his very own <mark>distributed-version-control-system</mark> that work quite fast & efficient. He wished to keep it free and [Open-Source](https://www.google.com/search?q=open+source+explained&sca_esv=9a0c77fca43723a5&sca_upv=1&rlz=1C1RXQR_enIN1070IN1070&sxsrf=ACQVn0-z4osJnKggLCAc5YFMHff6Kv1mqQ%3A1714708140032&ei=rF40Zu3QAde2vr0PrYqjqA8&oq=open-source+explaoned&gs_lp=Egxnd3Mtd2l6LXNlcnAiFW9wZW4tc291cmNlIGV4cGxhb25lZCoCCAAyBhAAGBYYHjIKEAAYBRgNGB4YDzIKEAAYBRgNGB4YDzIIEAAYCBgNGB4yCBAAGAgYDRgeMggQABgIGA0YHjIIEAAYCBgNGB4yCBAAGAgYDRgeMgoQABgIGA0YHhgPMgsQABiABBiGAxiKBUjlG1ApWPQOcAF4AJABAJgBuAGgAaAOqgEEMC4xMbgBAcgBAPgBAZgCC6ACyA3CAgoQABiwAxjWBBhHwgINEAAYgAQYsAMYQxiKBcICChAAGIAEGEMYigXCAgUQABiABMICBxAAGIAEGA3CAgYQABgNGB7CAggQABgWGB4YD8ICCBAAGAUYDRgemAMAiAYBkAYKkgcEMS4xMKAHlkw&sclient=gws-wiz-serp) for all the users globally.

Let's explore more about Git in further headings.

## Installation

**<mark>Git</mark>** <mark> : works as a software which is to be downloaded on Windows/ Mac/ Linux. </mark> [<mark>https://git-scm.com/</mark>](https://git-scm.com/)

> 💻 Video Tutorial to install Git for WINDOWS: [https://www.youtube.com/embed/nqCY3njHg2U?start=258&end=549](https://www.youtube.com/embed/nqCY3njHg2U?start=258&end=549)
> 
> 💻Video Tutorial to install Git for MaC : [https://www.youtube.com/embed/nqCY3njHg2U?start=607&end=813](https://www.youtube.com/embed/nqCY3njHg2U?start=607&end=813)

**GitHub**: could be optional to download. We've got it's website, desktop app as well as a mobile app to operate GitHub. It could be operated from any Browser or Operating System. [https://github.com/](https://github.com/)

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">Consider Git as <mark>VLC Media</mark> player- which only &amp; only operates on your computer, locally. Whereas, GitHub could be understood as <mark>Amazon Prime</mark><strong>.</strong> You can use it from it's website, desktop app, or even mobile app.</div>
</div>

---

# Why do we use [Git](https://www.youtube.com/embed/nqCY3njHg2U?start=1075&end=1569)?

> Big organizations like Microsoft, Apple, & Google, etc. have hundreds of employees working on the same project. Then how do they get to know 'who did which task?' [(detailed explanation here)](https://www.youtube.com/embed/nqCY3njHg2U?start=1075&end=1569)

Git is a distributed version-control system. That means it is used for <mark>tracking changes</mark> in the source code in software development.

It allows multiple developers to work on the same project and track every change, together. Git is called <mark>'distributed'</mark> because it gives it's users the flexibility to work independently, without relying upon a central server.

Here's a list of things Git can help us with. We can call them, **<mark>FEATURES OF GIT</mark>**

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714700993890/09fce14a-3ad6-427f-b247-d4f4e31a42ea.png align="center")](https://www.youtube.com/embed/nqCY3njHg2U?start=1569&end=1730)

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">Just like in Google Docs, each user gets tracked. Any type of change, done by any user is visible, with time-stamps. It stores the entire history of the document and every member that is working on it.</div>
</div>

Similar to this, we use Git for tracking all the changes from the first line of code, to the last one.

---

# Why is Git called version-control system?

Consider you are creating a Mobile App with a team of 4 members. Now, you decided to add a new feature i.e. a ChatBot to your app.

You and your team added it, but somehow it's not working- and you finally decide that you want to 'UNDO' your changes.

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">The Undo-Redo in software development is named as "Versioning" or "updating version". Hence, instead of saying "Undo changes", we actually say "back to the previous version".</div>
</div>

So, Git helps you to maintain versions of your code. And <mark>you can easily move to any version at any point of time (previous or next).</mark> Without Git, it becomes very tough to manually maintain every version, and move back to it!

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714701283893/ae8dad5e-efc9-482e-b91f-78d0d69ce04c.png align="center")](https://www.youtube.com/embed/nqCY3njHg2U?start=1738&end=1904)

---

# Understanding Stages within Git

As mentioned, you were working with your friends in a team of 4, and building a mobile app. Hence, in the technical terminology you are at the **<mark>WORKING DIRECTORY.</mark>**

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">WORKING DIRECTORY: the stage when you are working on your code- i.e. from the first line of code, till the last/recent changes. You will remain in the working directory until you're writing your code or making any changes.</div>
</div>

Now, once your code is ready, you would like to "SAVE" your changes. In software development we have a different way to 'save' or 'save as'.

> Saving changes in Git is a TWO-STEP process, similar as a 2-factor authentication of the Gmail account login.

If you'd like to save your changes, you will have to give the `git add .` command on the Git window (first step). After giving this command, your project will shift to **<mark>STAGGING AREA.</mark>**

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">STAGGING AREA: the stage where all your changes in the project are ready to be saved. In this stage, we give the name to the changes/work done on the project.</div>
</div>

Second step will to type `git commit -m "Name of the changes/work done"` command on the Git window. The message inside could be anything general that you've worked upon. For example "Added a chatbot" or "Updated the nav bar" etc. After this, your code files will successfully be called a **<mark>RESPOSITORY</mark>** now.

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">REPOSITORY: could be understood as kind of a project file that store versions and revision history along with it.</div>
</div>

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714703774735/338ae09d-7d08-40a2-964d-7495eff29961.png align="center")](https://www.youtube.com/embed/nqCY3njHg2U?start=1904&end=2228)

---

## Understanding by an Example

You might have worked on Microsoft Office Word. Right? And made a document by typing from the first line. If yes, then it'll be really easy for you to understand the <mark>working of Git with an example</mark>.

Well, whenever you typed the word document, you always save your changes. Similarly, for any update on code, you get to save it as soon as you're done adding it the the code. Git adds those changes, and doesn't overwrite over the last file, thereby updating a version of your code file.

[![Word 2013: Saving and Sharing Documents](https://media.gcflearnfree.org/ctassets/topics/233/save_export_2003_done2.png align="left")](https://www.youtube.com/embed/nqCY3njHg2U?start=1904&end=2228)

Now, in Microsoft Office Word, whenever we clicked on the 'Save' button or typed 'Ctrl+S' it take us to a pop-up window. It's the second step to select the location & entering the file name.

Similarly for Git, simply replace:

1. 'Ctrl+S' --&gt; `git add .`
    
2. 'Entering File Name' --&gt; `git commit -m "Name of the changes/work done"`
    

---

# How do we operate the Git window?

Good question! Because the git window interface actually looks like this:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714704745685/76417043-1aa8-4fa9-85c6-f89408177b38.png align="center")

But nothing to worry, as we've got a couple of commands to operate Git :

`git clone` , `git add .` , `git merge [branch]` , `git commit -m "[]"` , `git status` ,

`git fetch` , `git checkout` , `git push origin main` , `git pull` ....etc.

And all you need is to understand these commands without actually memorizing!

You can find the entire list of <mark>Git Commands</mark> from here: [https://education.github.com/git-cheat-sheet-education.pdf](https://education.github.com/git-cheat-sheet-education.pdf)

---

# Explaining the Git Commands

In this section, we will look for git terminology and it's commands- including their use case, and examples.

## git setup commands

In this, we basically tell the Git program (installed on our local machine, i.e. laptop/PC), the name of person who's making changes in the code.

First we tell the name, and then the email by:

`git config --global user.name "FirstName LastName"`*(press enter)*

`git config --global user.email "Your Email"`*(press enter)*

> *<mark>How to know if the Git command is working?</mark>*
> 
> *If your git command works successfully, it will straightaway take you to the next line. It only displays any text in case of an error. Watch this video snippet for understanding in detail :*[https://www.youtube.com/embed/nqCY3njHg2U?start=2451&end=2686](https://www.youtube.com/embed/nqCY3njHg2U?start=2451&end=2686)

## git init

With `git init`, we tell Git to <mark>initiate/start tracking the changes to the code files</mark> within it's directory. We use this command usually before making a new repository.

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">REPOSITORY: (or repo) could be understood as kind of a project file that store versions and revision history along with it.</div>
</div>

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">DIRECTORY is a folder on a computer system that stores files, providing a way to organize and manage data.</div>
</div>

(However, simply running `git init` doesn't automatically start tracking all files. You need to explicitly add files to the staging area using `git add` to start tracking them.)

## git clone

We use `git clone [url]` command in order to download an online repository to our local computer. For this, we need the URL link to that repository. It could be present on GitHub, GitLab, Bitbucket, or similar platforms.

[![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714944305497/5fbdd7f6-aa54-4ae8-9785-88d00800a6ca.png align="center")](https://github.com/trivedi-khushi)

Fun Fact: by "clone" we basically mean to "download" when we use Git.

```apache
git clone "https://github.com/trivedi-khushi/Portfolio-Website-demo-for-gdsc-upv.git"
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714946217173/7b154c22-098b-4b47-9537-1a1b65cfad8c.png align="center")

## git status

As the name suggests, `git status` tells you the <mark>status of your Git repository</mark>. The output possibility of this command could be :

* which files of your repo have been <mark>MODIFIED</mark> ,
    
* files that are <mark>STAGED</mark> (i.e. added to the next commit) ,
    
* & if any of those files are <mark>UNTRACKED</mark> (i.e. not yet added to Git's version control).
    

## git add

As we've seen before, this is the first step to 'save' changes in Git terminology. Well, `git add [File_Name]` is exactly like 'Ctrl+S' in MS Word, besides you need to mention the file name inside the Git command.

NOTE: <mark>if you need to save all the files, then you must enter </mark> `git add .` instead of file name. The <mark>dot in this command stands for 'all the files'</mark> that belongs to the repository.

> For Example: if the file name is '" hashnode.txt " then the git add command will be:

```abap
git add hashnode.txt
```

## [git commit](https://www.youtube.com/embed/nqCY3njHg2U?start=5135&end=5203)

This command is the second step while we save the code changes to the repository. `git commit -m "Your Message"` could be understood as a final confirmation of saving your changes, and you do this by giving a name to your changes. Just for example, "added the search bar", or :

```abap
git commit -m "Updated the CSS animation"
```

<mark>When you enter the </mark> `git commit` <mark> command, it means you've successfully added your changes &amp; input to the repository.</mark>

*Take it similar like you're adding a puzzle piece while solving it with your friends. Yeah, that's how you add your contribution to the overall code, like adding a piece.*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714947729839/787ec514-36f0-42b0-92ee-8692c40b2373.png align="center")

## git branch

Before knowing what this command actually does, we must understand the answer to ' what is a branch in git '. Well, branching <mark>helps developers to experiment a new feature on the software/project</mark> that is being built, by making a copy and not risking the original /source code. This is because we don't want to ruin the main code of the project, so we make a copy of it <mark>within the same repository.</mark> If the feature works on the copy, we merge it to the original branch of the code using 'pull requests'.

> Read this blog for more understanding: How is Branching (git branch) different from Forking on GitHub?

![What's the Best Git Merge Strategy?](https://blog.mergify.com/content/images/2021/04/Git-Branches-merge-stragegies.png align="left")

### **Didn't understand? Let's look into an example to understand** `git branch`

*Consider you made some a Soup for family dinner and it's less in some spices. Now, instead of adding any flavors /spices directly to the main soup, we try mixing seasonings, peppers, salt, and other spices to a bowl of soup, instead of the main soup pot. After it has been finalized which spices to be added, and which not - you will finally add the same proportion of selected flavors to the main soup pot.*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714951970724/17e4b91e-2e97-4aea-87d6-7884c4797dab.png align="center")

Similarly, we try to experiment, fix a bug, add a new feature, or bring a new color theme to our existing project. But, instead of risking the whole project for a little new edit, it's safe & better to get a copy of it to test it before adding it to the main & final copy of the code.

### Git Branch commands

There are mainly 4 branch commands that is used & mentioned in the [cheatseet](https://education.github.com/git-cheat-sheet-education.pdf).

1. `git branch` : used to see the list of all the existing branches of the repository.
    
2. `git branch [new-branch-name]` : it creates a new branch on the selected repo.
    
3. `git checkout` : it's used to checkout for the current branch you are in.
    
4. `git checkout [branch-name]` : it helps you to switch from the current branch to another existing branch of the repository.
    

> for any existing branch named "updates" we can enter:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714953301705/06e591ce-bf7b-4a85-b954-96ef6e697985.png align="center")

NOTE: There will always be one branch made automatically called "main". <mark>It is the default branch in any repository. Changes made in the '</mark>**<mark>main branch</mark>**<mark>' will be shown in the final overall output.</mark>

## [git merge](https://www.geeksforgeeks.org/git-merge/)

There is a command existing to merge the changes of one branch into another. We can enter the command : `git merge [branch-name]` in order to add the changes of `[branch-name]` into the branch that you're already working on.

NOTE: <mark>We can use this command to combine any branch with the main branch as well.</mark>

In that case, it'll be `git merge main` : (source- GeeksforGeeks.org)

[![Git - Merge - GeeksforGeeks](https://media.geeksforgeeks.org/wp-content/uploads/20230516192737/git-three-way-merging.png align="left")](https://www.geeksforgeeks.org/git-merge/)

## git pull

The Git Pull command is nothing but <mark>updating your local repo</mark> with the one that is existing at GitHub/ GitLab's platform.

After entering `git pull` the files in your local computer's repository will be updated with the files present in that URL link from where you initially cloned it in your system.

It will make the local repository as <mark>same as the remote repository</mark>.

## git push

<mark>'Push' in Git terminology could be understood as 'Upload'.</mark> This command is often written in a 4-word form like:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1714956335438/706305f4-e6b1-4870-85b8-a2e6bdf04fc3.png align="center")

Here, `git push origin main` means that we are uploading the changes made to the 'main' branch of the repository. The last word must be the branch name. Note: the git push command is only applicable for the existing branches of the repo.

> For instance, if we wanted to upload the code changes to an existing branch called "cloud-updates", then we get to enter the command as:

`git push origin cloud-updates`

## git fetch

This git command is used just for 'fetching' and downloading the information about the 'branched' from the original remote repository. `git fetch`

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">LOCAL repository means the project files/ repo present on your own PC.</div>
</div>

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">REMOTE repository refers to the repo present on the online development platform from where we initially cloned it using the URL.</div>
</div>

---

# Conclusion ❤️

I hope the very concept of a "distributed version-control-system" has been inclined well with the mentioned examples, and snippets.

***In the next write-up we will specifically look up to understanding how is Git (version-control) is different from the Open-Source development platforms like GitHub, GitLab, etc. ‼️***

In case of any queries, do reach out to [Khushi Trivedi](https://www.instagram.com/itni_khushii) 's socials mentioned. ❤️❤️

If this blogpost has been effective enough, do check out my other [**blogs**](https://hashnode.com/@KhushiTrivedi) and [**video contents**](https://www.youtube.com/channel/UCui5R0PVwnwPOkWS2YzepNQ) ✨