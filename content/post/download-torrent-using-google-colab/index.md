---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Download Torrent Using Google Colab"
subtitle: ""
summary: "Run this python notebook script to download torrent files in Google Colab"
authors: []
tags: []
categories: ["blog", "python"]
date: 2021-12-19T02:39:16-05:00
lastmod: 2021-12-19T02:39:16-05:00
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

Run this python notebook script to download torrent files in Google Colab.

<a href="https://colab.research.google.com/github/pollmix/google-colab-torrent-downloader/blob/master/torrent.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### Tutorial

Click the badge which says 'Open in Colab' and follow directions there.

### Purpose

1. Download torrent files where torrent downloading is restricted.
2. Make use of google servers download speed.
3. No installation of torrent softwares.
4. You only need a browser.

### Tutorial

1. Click the `Open in Colab` badge above.
2. Click `Runtime` -> `Run all`
   ![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/1.jpeg)
3. Input the torrent magnet link and press `Enter`
   ![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/2.jpeg)
4. Open `Files`. Press folder refresh icon. Your downloaded torrent file should be inside the `Torrent` folder
   ![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/3.jpeg)
5. Download the file by pressing right click -> `Download`
   ![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/6.jpeg)


### Notes

#### Google Colab files are temporary

One important caveat to remember while using Colab is that the files you upload to it won’t be available forever. Colab is a temporary environment with an idle timeout of 90 minutes and an absolute timeout of 12 hours. This means that the runtime will disconnect if it has remained idle for 90 minutes, or if it has been in use for 12 hours. On disconnection, you lose all your variables, states, installed packages, and files and will be connected to an entirely new and clean environment on reconnecting. [Source](https://neptune.ai/blog/google-colab-dealing-with-files)

#### Increase colab disk space

Google Colab gives 80GB space by default. But if you need more space around 350GB then click Runtime -> Change runtime type and give GPU as the Hardware Accelerator.

![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/4.jpeg)

![](https://github.com/pollmix/google-colab-torrent-downloader/raw/master/img/5.jpeg)

#### Redownload missing files
If somehow some files are missing try to re-download torrent by rerunning the script. Fastresume will check files.
