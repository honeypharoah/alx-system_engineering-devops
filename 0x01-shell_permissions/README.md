# Shell Permissions

## My Name is Betty
- Create a script that switches the current user to the user
- `su new.username`

## Who Am I
- Write a script that prints the effective username of the current user
- `whoami`

## Groups
- Write a script that prints all the groups the current user is part of.
- `groups` or `id -Gn`

## New Owner
- Write a script that changes the owner of the file hello to the user betty.
- `chown username filename`

## Empty
- Write a script that creates an empty file called hello.
- `touch filename`

## Execute
- Write a script that adds execute permission to the owner of the file hello.
- `chmod u+x filename` 

- where u = user and x = execute 

## Multiple Permissions
- Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
- `chmod u+x,g+x,o+r filename`
 
- where g = group, o = other and r = read

## Everybody
- Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
- `chmod a+x filename` or `chmod +x filename` 

## James Bond
- Write a script that sets the permission to the file hello as follows: Owner no permission at all, Group no permission at all, Other users: all the permissions 
- `chmod 007 filename`

## John Doe
- Write a script that sets the mode of the file hello to this: -rwxr-x-wx
- `chmod 753 filename`

## Look in the Mirror
- Write a script that sets the mode of the file hello the same as olleh’s mode.
- `chmod --reference=olleh hello`

## Directories
- Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.
- `chmod -R +X *` or `chmod -R a+X *` 

- where R applies the change recursively - to all directories within the current working directory, X executes directories only and * is a wil  

## More Directories
- Create a script that creates a directory called my_dir with permissions 751 in the working directory.
- `mkdir -m 751 my_dir` where m = mode 

## Change Group
- Write a script that changes the group owner to school for the file hello
- `chown owner:new.group.owner filename` --> `chown root:school hello`

## Owner and Group
- Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
- `chown vincent:staff *`

## Symbolic Links
- Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.
- `chown -h vincent:staff hello`

## If Only
- Write a script that changes the owner of the file hello to betty only if it is owned by the user guillaume.
- `chown -from=guillaume betty`

## Star Wars
- Write a script that will play the StarWars IV episode in the terminal.
- `telnet towel.blinkenlights.nl`

