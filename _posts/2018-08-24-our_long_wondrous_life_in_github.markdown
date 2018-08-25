---
layout: post
title:      "Our Long Wondrous Life in GitHub "
date:       2018-08-24 22:31:28 -0400
permalink:  our_long_wondrous_life_in_github
---


As we start our careers in Software Engineering, GitHub becomes our second resume. To make the GitHub experience that much more wondrous, here are some git commands to keep at bay:

**want to create a new local repository?**
```
git init
```


**want to check out a repository?**   

*create a copy of a local repo:*
```
git clone /path/to/repo
```

*or for a remote server:*
```
git clone ssh-key
```


**want to add files to staging?**   

*add one file:*
```
git add filename
```

*add all files:*
```
git add *
```


**want to check the status of your files?**
```
git status
```


**want to commit changes? (not to the remote repo)**
``` 
git commit -m "message"
```


**want to push changes? (to the remote repo)**
```
git push origin master
```

On the surface git commands may seem to be easy to execute but there are other situations that can arise that require more triaging on what went wrong and how to fix it. 

**want more basic git commands to reference?**
[Git Cheat Sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)

*Happy GitHubbin' to all!*


