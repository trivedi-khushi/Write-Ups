---
title: "Advanced GIT - Top 6 Version Control Hacks That Saves You Time"
seoTitle: "Git Version Control: Top 6 Time-Saving Hacks"
seoDescription: "Top six Git & GitHub command hacks to save your hours"
datePublished: Tue Jan 07 2025 04:58:40 GMT+0000 (Coordinated Universal Time)
cuid: cm5m032iz000009mbfztjclt3
slug: advanced-git-top-6-version-control-hacks-that-saves-you-time
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1736224502853/9c5dd07c-ad12-47ee-a526-0b245e75c1d6.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1736225890960/a04cdab5-284b-4a50-ad1b-75dd0049e353.png
tags: hackathon, github, technology, version-control, community, git, hacking, tech, hashnode, hacks, pull-requests, gitcommands, advanced-git, version-control-systems, khushitrivedi

---

Here we are with another blog featuring **Git**. My previous write-up on version-control showed a pretty good response- which was a beginner-guide to learn the basics of Git Commands and Controls.

Well, this blog is about some Git-Productivity hacks which helped me save hours. Take a look yourself!

## 1\. Clone only a specific branch of the repository

While cloning any repo from GitHub, we directly download the main (default) branch to our systems. Here’s what we can do in-case we’re preferring any specific branch:

**SYNTAX :** `git clone --single-branch -b <branch-name> "<repo-link>"`

**EXAMPLE :** In case we’d like to clone a specific branch named “fix-blog-links” from Appwrite’s GitHub Repository, we can use this command on our terminal

`git clone --single-branch -b fix-blog-links “`[`https://github.com/appwrite/appwrite.git`](https://github.com/appwrite/appwrite.git)`”`

---

## 2\. Link your PR to any Issue

We can actually link Pull requests with any GitHub Issue. Plus, we can automatically close that issue by just editing our PR’s description or comment. Here’s how we do it:

* ### **Link the issue within the same repo:** (in which you’re raising the PR)
    
    **SYNTAX :** `<your-keyword> #issue-number`
    
    **EXAMPLE :** `Closes #9` , `fixed #13`
    
* ### **Link the issue which is on a different repository:**
    
    **SYNTAX :** `keyword <repo-owner>/<repo-name>#issue-number`
    
    **EXAMPLE :** In-case of a repository name: portfolio, and the owner: [trivedi-khushi](https://www.github.com/trivedi-khushi) we can mention the comment as: `fixes portfolio/trivedi-khushi#5` in which, 5 indicates the issue number on the portfolio repository.
    
* ### **Link the Multiple Issues:**
    
    **SYNTAX :** use full syntax for each issue, and separate it by comma `,`
    
    **EXAMPLE :** `resolves #149, resolves #6, resolves portfolio/trivedi-khushi#7`
    

---

## 3\. Search within your entire Git Histroy

Ever wanted to search throughout your commit history for a specific keyword? We can actually do it by adding a `-S` flag to the `git log` command. It’s certainly more than what a normal text search (Ctrl+F) could do.

**Using this comamnd, we can view all the additions and deletions made throughout the code changes** in the Git Commit History. Also, this search command is **case-sensitive,** so make sure to type in the correct string while searching.

**SYNTAX :** `git log -S "<your-keyword>"`

**EXAMPLES :** `git log -S "initializeDatabase"`

If you understood the purpose of the search command, it would be interesting to know about:

* **Search within a range of commits:** We can easily use an updated command `git log -S “<your-keyword>” <start-commit>..<end-commit>`. A simple example for this could be: `git log -S "initializeDatabase" HEAD~10..HEAD`
    
* **Search Within any Specific File:** Here’s a syntax in order to search based on your specific file: `git log -S <your-keyword> -- <file-path>`. This command comes with a disadvantage of not supporting files after their rename. For that, we can specifically use a `-follow` flag to this command. For instance, `git log -S "initializeDatabase" --follow -- path/to/file`.
    

---

## 4\. Tag any Specific Commit

Tags in Git could be used in order to part a couple of places to be important within your project. We can use tags for any reason such as:

* releases,
    
* feature-complete,
    
* experiemntal feature,
    
* milestone, etc.
    

Well, you can only use tagging in Git if you’ve already made a commit. Here’s how we can use git tag on our terminal:

**SYNTAX :** `git tag <tag-name> <commit-id>`

**EXAMPLE :** Let’s consider tagging a commit to remember it with first release. We can use: `git tag v1.0 1a2b3c4`

---

## 5\. List Remote Branches without Cloning them

We can easily list down the branches within a repository without cloning any of them. However, this only list down branch-names and not their contents like branch-specific files/folders.

**SYNTAX :** `git ls-remote --heads <repo-link>`

**EXAMPLE :** `git ls-remote --heads` [`https://github.com/appwrite/appwrite.git`](https://github.com/appwrite/appwrite.git)

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">No, <strong>double quotes</strong> are not required for the repository link in the <code>git ls-remote</code> command unless the link contains special characters or spaces (which is rare in Git URLs).</div>
</div>

---

## 6\. Undo any Local Commit

We can easily undo a Local Commit made, without losing any changes. Here’s how we do it:

**SYNTAX :** `git reset --soft HEAD~1`.

The flag here `--soft` removes the changes from the commit, but they will be still present in the staging area. We can use this to rather remake suitable chnages and commit later. Meanwhile, `HEAD~1` indicates most recent commit done (the one we’re undoing).

---

Hope it added value for you. There’s no particular source where these all could be found listed. so, feel free to comment any other hacks you use.If these hacks were impressive, and the blog was a nice resource for you, make sure to support me by following my [hashnode profile](https://hashnode.com/@trivedi-khushi)!❤️