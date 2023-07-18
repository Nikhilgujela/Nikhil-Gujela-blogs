---
title: "Day 2 : Basics Linux Commands with Examples"
datePublished: Tue Jul 18 2023 05:01:31 GMT+0000 (Coordinated Universal Time)
cuid: clk7tukj5000609lebchu1kfh
slug: day-2-basics-linux-commands-with-examples
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689591702399/2025215d-20db-4c50-98cb-654a742ebb70.png
tags: cloud, linux, aws, devops, 90daysofdevops

---

## **Introduction:**

Linux is an operating system that is highly favored by tech enthusiasts because of its powerful features. It provides a wide range of command-line tools that are useful for various tasks. In this blog, we'll cover three fundamental Linux commands that are easy to understand even for beginners. These commands include checking the current working directory, displaying files and directories (including hidden files), and creating nested directories. So, let's get started and explore the Linux command line! 🚀

## Task 1: Checking Your Current Location 📂

Command: `pwd`

* The `pwd` command shows you the directory you're currently in, like a GPS for your computer.
    
* It displays the full path of the directory you're working in.
    
* Directories are "Folders" in Linux
    

Example: If your current directory is `/root/newfolder`, running `pwd` will show `/root/newfolder` in the terminal.

```bash
ubuntu $ pwd
/root/newfolder
```

## Task 2: Listing Files and Directories, Including Hidden Files 📋

Commands : `ls -a`

* The `ls` command lists files and directories.
    
* Adding the `-a` option shows hidden files and directories. In Linux, hidden files start with a dot (e.g., `.config`).
    
* Adding the `-la` option shows hidden files and directories with more details.
    
    (e.g., permission, owner, group, creation date, etc.)
    
* This command gives you a complete view of all files and directories in the current location.
    

Example: Running `ls -a` in a directory will display a list of all files and directories, including hidden ones, in the terminal output.

```bash
ubuntu $ ls 
file1.txt  file2.txt
ubuntu $ ls -a
.  ..  file1.txt  file2.txt
ubuntu $ ls -la
total 8
drwxr-xr-x 2 root root 4096 Jul 17 11:54 .
drwx------ 5 root root 4096 Jul 17 11:53 ..
-rw-r--r-- 1 root root    0 Jul 17 11:54 file1.txt
-rw-r--r-- 1 root root    0 Jul 17 11:54 file2.txt
```

## Task 3: Creating a Nested Directory / Directory inside Directory 🗂️

Command: `mkdir -p A/B/C/D/E`

* The `mkdir` command is used to create directories.
    
* The `-p` option ensures that parent directories are created if they don't exist. This allows for creating a nested directory structure with a single command.
    

Example: Running `mkdir -p A/B/C/D/E` will create the following nested directory structure:

<mark>Note: </mark> **"tree"** command is used to see the files & folders from the current directory.

```bash
ubuntu $ mkdir -p A/B/C/D/E
ubuntu $ tree
.
|-- A
|   `-- B
|       `-- C
|           `-- D
|               `-- E
|-- file1.txt
`-- file2.txt
```

## Conclusion:

In summary, don't be intimidated by the Linux command line. With a few key commands such as pwd, ls -a, and mkdir -p, you can quickly become comfortable with the system. These commands are essential for exploring Linux and unlocking its full potential. So, don't hesitate to embrace the command line and begin your journey into the world of Linux! 🐧🌟