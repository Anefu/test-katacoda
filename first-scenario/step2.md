# Files and Filesystem
### ls Command
**ls** lists the contents of a directory.  
You can pass in various flags to the **ls** command, depending on what you want to do.  
First let's create some files  

`touch darey katie john`{{execute}}  
Now execute ls to see the files you created (typing ls alone displays the content of the directory you're in)  
`ls`{{execute}}  
Create more files in the same directory (using the **touch** command above which creates empty files)

To list all the contents including hidden files and directories, use the '-a' flag  
`ls -a`{{execute}}
  
To list contents, sorted newest first, use the '-t' flag  
`ls -t`{{execute}}  
  
You can also combine flags. The example below does a listing of all the files sorted by the time they were created  
`ls -at`{{execute}}  

  
### mkdir Command
**mkdir** (a concatenation of the words **make** and **directory**) is used to create directories on your system.  
  
Click:  
`mkdir darey.io`{{execute}}  
To make the directory (or any file) hidden, its name should start with a **.**.  
`mkdir .linux`{{execute}}  
  
Now you've learned how to create directories, but how do you enter them?
### The cd Command
**cd** (change directory) moves you in the directory you specify.  
Running cd with any options just returns you back to the home directory of your current user.  
Some examples for you:  
  
`cd darey.io`{{execute}}

### The cp Command
**cp** (short for **copy**) does what its name implies; copies files! (That rhymes by the way)  
The **cp** command also copy directories (use the -r flag to recursively copy the contents of the directory too). For example:  
  
Check your current directory using pwd  
`pwd`{{execute}}  
  
Now cd back to the previous directory  
`cd ..`{{execute}}  
  
Try out your first copy command  
`cp darey darey.io/`{{execute}}  
  
The first argument describes the file (or directory) you want to copy, the second argument defines its destinatio.  
You can copy multiple files to the same destination by specifying the files first and the destination last. For example:  
`cp katie john darey.io/`{{execute}}