---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Add Remote Git Repository"
subtitle: ""
summary: "Add a new remote repository to a local Git repository"
authors: []
tags: ["git"]
categories: []
date: 2022-05-28T06:51:23-04:00
lastmod: 2022-05-28T06:51:23-04:00
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

`git remote add` is a command used in Git version control system to add a new remote repository to a local Git repository.

Here's the basic syntax of the `git remote add` command:

```bash
git remote add <remote-name> <remote-url>
```

- `<remote-name>` is the name you want to give to the remote repository. This is typically set to `origin`.
- `<remote-url>` is the URL of the remote repository you want to add.

For example, if you want to add a remote repository with the name `origin` and the URL `https://github.com/username/repo.git`, you would run the following command:

```bash
git remote add origin https://github.com/username/repo.git
```

Once you've added a remote repository, you can use other Git commands like `git push` and `git fetch` to interact with the remote repository.
