---
title: "Day 3 : Basic Linux Commands"
datePublished: Wed Jul 19 2023 04:32:28 GMT+0000 (Coordinated Universal Time)
cuid: clk9892a4000d0ami5x3r8lpx
slug: day-3-basic-linux-commands
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1689596011607/4805f995-ee5f-48ed-8ef9-8c5bb3aa16b6.png
tags: linux, aws, azure, devops, 90daysofdevops

---

## Introduction:

Linux commands are tools that can help users navigate and manage the file system with efficiency. This blog is designed for beginners and will cover a variety of essential Linux commands that can be used for common tasks. Whether you want to view the content of a file or create and modify directories, we'll explore the power of the Linux command line together. 🚀

## Task 1: Viewing the Content of a File 👀

Command: `cat filename`

* The `cat` command displays the content of a file on the terminal.
    
* By specifying the `filename`, you can view the entire content of the file in one go.
    

Example: To view the contents of a file called `file.txt`, run:

```bash
$ cat file.txt
```

## Task 2: Changing the Access Permissions of Files 🔐

Command: `chmod permissions filename`

* The `chmod` command allows you to modify the access permissions of a file or directory.
    
* `permissions` can be represented in numeric or symbolic form, specifying read (`r`), write (`w`), and execute (`x`) permissions for the owner, group, and others.
    
* r (read): 4
    
    w (write): 2
    
    x (execute): 1
    

**Example:** To change the permissions of `file.txt` to read, write, execute for the owner and read-only for others, run:

Previous permission: rw-r--r--

```bash
$ ls -l
-rw-r--r-- 1 root root 39 Jul 17 11:34 file.txt
```

Current permission: rwxr--r--

```bash
$ chmod 744 file.txt
$ ls -l
-rwxr--r-- 1 root root   39 Jul 17 11:34 file.txt
```

## Task 3: Checking Your Command History 📚

Command: `history`

* The `history` command displays a list of commands you have executed previously.
    
* It provides a helpful reference to track your past interactions with the Linux command line.
    

Example: To view the command history, simply run:

```bash
$ history
```

## Task 4: Removing a Directory/Folder 🗑️

Command: `rm -r directory_name`

* The `rm` command is used to remove files and directories.
    
* Adding the `-r` option allows you to delete a directory and its contents recursively.
    

Example: To remove a directory named `newfolder`, run:

```bash
$ rm -r newfolder/
```

## Task 5: Creating and Viewing the Content of a File 📝

Commands:

* `touch` creates a new file, `fruits.txt`, if it doesn't exist.
    
* `echo` appends the specified content to `fruits.txt`, with each fruit on a new line.
    
* `cat` displays the content of `fruits.txt` on the terminal.
    

```bash
$ touch fruits.txt
$ echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > fruits.txt
$ cat fruits.txt
```

## Task 6: Adding Content to a File Line by Line 🖋️

Command: `echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > fruits.txt`

* `echo` appends the specified content to `fruits.txt`, with each fruit on a new line.
    

Example: To add the fruits "Apple," "Mango," "Banana," and others to a file named `fruits.txt`, run:

```bash
$ echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > fruits.txt
$ cat fruits.txt
```

## Task 7: Showing Only the Top Three Fruits from the File 🥇

Command: `head -n 3 fruits.txt`

* The `head` command displays the top lines of a file.
    
* Adding the `-n 3` option shows only the first three lines of the file.
    

Example: To display the top three fruits from `fruits.txt`, run:

```bash
$ head -n 3 fruits.txt
```

## Task 8: Showing Only the Bottom Three Fruits from the File 🥉

Command: `tail -n 3 fruits.txt`

* The `tail` command displays the last lines of a file.
    
* Adding the `-n 3` option shows only the last three lines of the file.
    

Example: To display the bottom three fruits from `fruits.txt`, run:

```bash
$ tail -n 3 fruits.txt
```

## Task 9: Creating and Viewing the Content of Another File 🌈

Commands:

* `touch` creates a new file, `colors.txt`, if it doesn't exist.
    
* `echo` appends the specified content to `colors.txt`, with each color on a new line.
    
* `cat` displays the content of `colors.txt` on the terminal.
    

```bash
$ touch colors.txt
$ echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > colors.txt
$ cat colors.txt
```

## Task 10: Finding the Difference Between Two Files 🔄

Command: `diff file1.txt file2.txt`

* The `diff` command compares the contents of two files and displays the differences, if any.
    

Example: To find the difference between `fruits.txt` and `colors.txt`, run:

```bash
$ diff fruits.txt colors.txt
```

## Conclusion:

Linux commands provide users with the ability to carry out different tasks with ease and efficiency. These commands are essential for mastering the Linux command line, allowing users to view file content, modify permissions, create and manipulate files and directories. By experimenting and exploring these commands, users can become proficient in utilizing Linux's power and completing their tasks like an expert.🐧🌟