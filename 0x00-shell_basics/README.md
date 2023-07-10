# SHELL BASICS

## Where am I?
- Write a script that prints the absolute path name of the current working directory 
- ` pwd `

## What's in there?
- Display the contents list of your current directory 
- ` ls `

## There is No Place Like Home
- Write a script that changes the working directory to the user’s home directory 
- ` cd `	

## The Long Format
- Display current directory contents in a long format 
- ` ls -l `

## Hidden Files
- Display current directory contents, including hidden files 
- ` ls -a `

## I Love Numbers
- Display current directory contents in long format with user and group IDs displayed numerically 
- ` ls -lna `

## Welcome
- Create a script that creates a directory named dir2 in the /dir/ 
- ` mkdir /dir1/dir2 `

## Betty in My First Directory
- Move the file1 from /dir1/ to /dir1/dir2 
- ` mv /dir1/file1 /dir1/dir2 `

## Bye Bye Betty
- Delete file1 
- ` rm /dir1/dir2/file1 `

## Bye Bye My First Directory
- Delete dir2 that is in dir1 
- ` rmdir /dir1/dir2 `

## Back to the Future
- Write a script that changes the working directory to the previous one 
- ` cd - `

## Lists
- Write a script that lists all files in the current directory and the parent of the working directory and the dir3 (in this order), in long format 
- ` ls -la . .. /dir3 `

## File Type 
- Write a script that prints the type of the file named file2 in /dir1 
- ` file /dir1/file2 `

## We are Symbols, and Inhabit Symbols
- Create a symbolic link to /bin/ls named _link_, in the current working directory 
- ` ln -s /bin/ls _link_ `

## Copy HTML Files
- Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory 
- ` cp *.html ../ `

## Lets Move 
- Create a script that moves all files beginning with an uppercase letter to the directory /dir1/dir3 
- ` mv [[:upper:]]* /dir1/dir3 `

## Clean Emacs
- Create a script that deletes all files in the current working directory that end with the character ~ 
- ` rm *~ `

## Tree
- Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory 
- ` mkdir -p welcome/to/school `

## Life is a Series of Commas, Not Periods
- Write a command that lists all the files and directories of the current directory, separated by commas (,), directory names should end with a slash, hidden files listed, alpha ordered/digits first 
- ` ls -xamp `

## File Type: School
- Create a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset
- ` 0 string SCHOOL School data\n !:mime School --> file -C -m `
- where C means to compile 



