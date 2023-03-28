---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "How to Run a Java Project Using Eclipse IDE - step by step"
subtitle: ""
summary: "Run a new Java project by following all prerequisites shown with images"
authors: []
tags: ["java"]
categories: ["java"]
date: 2021-12-19
lastmod: 2021-12-19
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

{{% toc %}}

## Download and install Java

The first step is to download a JDK (Java Development Kit). You can search for "Java JDK download"
or [click this link](https://www.oracle.com/java/technologies/downloads/) to download Java.

Download the package for your operating system. For me, I am running windows so I will download the
x64 Installer for my pc.

Running the installer.
![Java Installation](installer-min.jpeg "Java Installation")
![Java Installation](installer2-min.jpeg "Java Installation")

> Note: Now Eclipse provide JRE installation while installting the IDE, so downloading JDK from oracle
> is not necessery. But, for backward compability, we are going to use oracle provided JDK.

## Download and install Eclipse

We need an IDE (Integrated Development Environment aka code editor) to write our first Java program.
We will use Eclipse IDE. You can download the software [from here](https://www.eclipse.org/downloads/).

After download, install the software.

Selecet Eclipse IDE for Jada Developers.
![Eclipse Installation](eclipse-installation-min.jpeg "Eclipse Installation")

As we installed JDK earlier, Eclipse will automatically pick out installed JDK.
![Eclipse Installation](eclipse-installation2-min.jpeg "Eclipse Installation")

However, if you wish you can pick up other JRE provided by Eclipse.
![](alternative-jvm-min.jpeg)

Continue installation by Accepting terms and conditions.
![Eclipse Installation](eclipse-installation3-min.jpeg "Eclipse Installation")

You can change the default directory for new projects.
![](workspace-min.jpeg)


## Create and run a new project
Open Eclipse by searching on windows.
![](open-min.jpeg)

Create a new Java project.
![](new-java-project-min.jpeg)

For the project I want to use the default location, use a project specific JRE and don't want
to create `module-info.java` file.
![](project-name-min.jpeg)

Now, I want to create a `Main` class.
![](new-class-min.jpeg)

I want to generate a `public static void main` method me.
![](main-class-min.jpeg)

I have added the de facto `Hello World` print. Now, time to run the program.
![](run-min.jpeg)

I always prefer to save the files before running the project.
![](save-min.jpeg)

Atlast, out disired output is here
![](output-min.jpeg)

Hope now you have a clear idea how to create a new project.

