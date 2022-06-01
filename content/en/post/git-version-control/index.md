---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Version control. Git."
subtitle: "How version control works, in particular Git."
authors: []
tags: []
categories: []
date: 2022-05-05T19:12:32+03:00
lastmod: 2022-05-05T19:12:32+03:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

## What's a git?

Git is a distributed version control system. It was developed by Linus Torvalds to manage the development of the Linux kernel.

## And what is a version control system?

A version control system is a software that allows you to store multiple versions of the same document and, if necessary, go back to past versions, merge them, track changes, and much more. Thus, the version control system greatly facilitates work both with large projects, in which there are many "blocks" and modules that are developed separately, and with single files, for example text documents, in which you can return to any version of previously written text.

## How does it work?

### Repository as a project

In git, the "project unit" is the repository. It's like a kind of directory that stores files, versions and everything related.

### Branches

In git, there is a concept of "branches" that divide the entire flow of changes made and the entire project as a whole into different "currents". Thus, you can make separate branches for individual innovations, separate pre-release versions (beta versions) and for any other conditional divisions.

### Client-server

git is initially installed as a local utility, but it can also be used in conjunction with the server. In this case, local changes will need to be uploaded to the server, which will be a centralized "point of truth" (i.e., where the most up-to-date version of the project is located). This also gives the advantages of saving data, that in case the local version disappears, the version on the server will serve as a backup.

## Why?

After talking about git as a system, it's worth understanding what benefits it can bring to you. 

I think everyone has already identified the main point for themselves that this allows you to control work on something much more flexibly and conveniently. However, let's mention a few more advantages of the git version control system.

### General work

In the scenario of using git together with the server, it opens up the possibility of several users working on one project. In this case, everyone is working on their part of the project, uploads it to the repository and there it is all assembled into a single project. If conflicts arise, they can be resolved in such ways as merge or choosing a priority version.

### "Packaging" of the code

When using git, it is possible to create so-called "packages". This is a "assembled" project that is distributed as a ready-made version. In the case of some program, it will be an executable file.

### Pipeline (CI/CD)

Also (most likely in a scenario with a server for git) it is possible to create a so-called development pipeline. I.e., you can configure the rules by which, when certain events trigger (for example, uploading a new commit to the *dev* branch), the processing process will be performed. Continuing the example, when loading a new commit (code), all tests will be performed and an attempt will be made to run the program on various operating systems, which will allow you to check the operability of the code and its maintainability.


In conclusion, I would like to say that everyone should at least try using git. Believe me, you will like it!
