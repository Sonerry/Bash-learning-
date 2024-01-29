## Some basic bash commands
``` bash
pwd
mkdir
cd
rm
echo
touch
cat
rm  
cp
mv
```

let's get started then
## pwd command
The pwd command shows the name of the directory you are in and prints the working directory.
``` bash
└─yourname@hostname$ pwd  
/home/yourname                                                   	
```
 
> [!UYARI]
> When we first log in to our system (or start a terminal emulator session) our current working directory is set to our home directory. Each user account is given its own home directory and it is the only place a regular user is allowed to write files. 

### !!some commands to guide you:+1:

``` bash
└─yourname@hostname$ man  pwd      
```
[ What is 'man' ](https://en.wikipedia.org/wiki/Man_page)
Is the terminal dirty?

``` bash
└─yourname@hostname$ clear                                                 	
```
``` bash
└─yourname@hostname$ man man
what it this ?                              	
```
```bash
 └─yourname@hostname$ whatis this                                                   	
```
Let's create a folder for our workspace

```bash
 └─yourname@hostname$ # This comment and Let's create the test directory make directory
 └─yourname@hostname$ mkdir  test
 └─yourname@hostname$ #  Congratulations, we created a new folder, let's enter the directory                           
```
If you want to create two directories.okay but why ? Some things have no reason :confused:

```bash
└─yourname@hostname$ mkdir for_you for_me 
```                               	 
:point_right::point_left:  
How to delete these directories? Are you really going to delete them?
```bash
└─yourname@hostname$ cd  test
└─yourname@hostname$ # cd change directory.We are now in the test directory. 
└─yourname@hostname$ pwd  
	 /home/yourname/test
```                                      	  
 Remember
  

Let's create a file in the test directory. What else can be done in a directory?
 > [!İMPORTANT] 
 > Filenames and commands in Linux, like Unix, are case sensitive. The filenames “File1” and
 “file1” refer to different files

```bash
└─yourname@hostname$ touch hello_world.txt 
└─yourname@hostname$ #Great job.So how to create three files?
└─yourname@hostname$ touch welcome.txt to.txt bash.txt    
```

hmm, have these files been created?  Are you sure? :thinking: Get ready, a new command is coming.

```bash
└─yourname@hostname$ ls  #ls list.Lists files or directories in the current directory
└─yourname@hostname$ bash.txt hello_world.txt to.txt welcome.txt 
```

 Let's play around with the ls command
```bash
└─yourname@hostname$ ls -l -a # The -l parameter means long and the -a parameter means all.
└─yourname@hostname$ # or ls -la ; ls-al; ls -a -l These are all the same.
└─yourname@hostname$ # try these commands and see the difference ls -a ; ls -l
└─yourname@hostname$ 
total 8
drwxr-xr-x 2 root root 145 Jan 29 19:43 .
dr-xr-x--- 3 root root 264 Dec 26 2020 ..
-rw-r--r-- 1 root root 0 Jan 29 19:44 bash.txt
-rw-r--r-- 1 root root 0 Jan 29 19:43 hello_world.txt
-rw-r--r-- 1 root root 0 Jan 29 19:44 to.txt
-rw-r--r-- 1 root root 0 Jan 29 19:44 welcome.txt
```

What is going on here?
## . and.. what are they

. directory we are in.
.. previous directory, in our case /home/yourname

```bash
└─yourname@hostname$ cd  ..
└─yourname@hostname$ pwd  #/home/yourname
└─yourname@hostname$ cd  test                                  	
```
I will explain the others in the chmod command. For now, just know that this is about file permissions.
In the meantime, we can do the above commands as follows:
``` bash
└─yourname@hostname$ cd  ..  ;  pwd                               	
```
For now, let's clean up this dirty area.
``` bash
└─yourname@hostname$ rmdir  test  #delete test directory                               	
```
see you in the next lesson.