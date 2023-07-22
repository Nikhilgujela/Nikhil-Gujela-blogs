---
title: "Day 4 : Basic Linux Shell Scripting for DevOps Engineers."
datePublished: Sat Jul 22 2023 07:33:25 GMT+0000 (Coordinated Universal Time)
cuid: clkdp1c2h000d09mgbrxt2ro8
slug: day-4-basic-linux-shell-scripting-for-devops-engineers
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1690010893784/ec57ff75-acc3-4b81-9809-cff6fdd1160e.png
tags: linux, aws, devops, shell-scripting, 90daysofdevops

---

## Introduction:

Shell scripting is an incredibly useful tool for DevOps professionals, as it allows them to automate repetitive tasks, simplify processes, and increase productivity. In this blog post, we will delve into the fundamentals of shell scripting, such as its key elements, the process of writing a simple script, and various examples of utilizing conditional statements. So, let's jump right into the realm of automation with shell scripting! 🚀

## What is Shell Scripting for DevOps? 🐚

* Shell scripting is a method of creating and executing scripts using command-line interpreters (shells) in Unix-like operating systems.
    
* For DevOps professionals, shell scripting is a key element in automating routine tasks, managing infrastructure, and facilitating continuous integration and deployment (CI/CD) pipelines.
    

## What is #!/bin/bash? Can we write #!/bin/sh as well? 🤔

* `#!/bin/bash` is called a "shebang" and appears at the beginning of a shell script.
    
* It tells the system which shell to use when executing the script. In this case, it specifies the Bash shell.
    
* Yes, you can use `#!/bin/sh` as well, which represents the system's default shell. However, using `#!/bin/bash` ensures consistent behavior across different systems.
    

## Writing a Shell Script for the #90DaysOfDevOps Challenge 📝

```bash
#!/bin/bash

# This script prints a motivational message for the #90DaysOfDevOps challenge
echo "I will complete the #90DaysOfDevOps challenge!"
```

* Save the script in a file, e.g., `devops_challenge.sh`.
    
* Make the script executable with the command: `chmod +x devops_challenge.sh`.
    
* Execute the script with: `./devops_challenge.sh`.
    

## Write a Shell Script to take user input, input from arguments and print the variables. 📥

```bash
#!/bin/bash

# Taking user input
echo "Please enter your name:"
read name
echo "Hello, $name! Welcome to the DevOps world."
```

* Save the script in a file, e.g., `user_input.sh`.
    
* Make the script executable with the command: `chmod +x user_input.sh`.
    
* Execute the script with: `./user_input.sh John Doe`.
    

## Example of If Else in Shell Scripting by Comparing Two Numbers 🔄

```bash
#!/bin/bash

# Taking user input
echo "Enter your first no :"
read num1
echo "Enter your second  no : "
read num2

# Comparing two numbers using if else
if [ $num1 -gt $num2 ]; then
    echo "$num1 is greater than $num2."
elif [ $num1 -lt $num2 ]; then
    echo "$num1 is less than $num2."
else
    echo "$num1 and $num2 are equal."
fi
```

* Save the script in a file, e.g., `compare_numbers.sh`.
    
* Make the script executable with the command: `chmod +x compare_numbers.sh`.
    
* Execute the script with: `./compare_numbers.sh`.
    

## Conclusion:

Shell scripting is a fundamental skill for DevOps professionals, enabling them to automate tasks and enhance efficiency. By creating scripts, you can streamline repetitive actions, interact with users, and make data-driven decisions using conditional statements. With the power of shell scripting, DevOps practitioners can focus on innovation and building robust, scalable systems to drive their projects forward. Embrace the world of automation with shell scripting and conquer the DevOps landscape! 🐚🌟