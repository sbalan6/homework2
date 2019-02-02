# Homework 2 - A Simple Shell Pt. 1
## Due: 14 February 2019
### Introduction
In our time here at UIC, we've all been working in the BASH shell for a good portion of our assignments, but have you ever thought about how it works? [BASH](https://en.wikipedia.org/wiki/Bash_(Unix_shell), has some powerful features! BASH is based on the [Bourne Shell](https://en.wikipedia.org/wiki/Bourne_shell) which might make Stephen Bourne cooler than Jason Bourne in my book!

### Assignment
For part one of this multi-part assignment we'll be implementing a very simple shell. Your shell should be able to execute commands in the foreground. 
```bash
cs361 > <command> list of arguments
<command> does its thing
pid: xxxxx status: y
cs361 >
```
Requirements
-[ ] Launch a process from the command and pass it a list of arguments
-[ ] Wait for command to exit
-[ ] Display the pid of the finished process and its exit status

Your shell should be able to launch commands in the background
```bash
cs361 > <command> list of arguments &
[1] pid
cs361 > fg
<command> is active and finishes
cs361 >
```
-[ ] Launch a process from the command and pass it a list of arguments
-[ ] Run the process in the background
-[ ] Bring the process to foreground using fg

The shell must run repeatedly until the user types exit at the command line. 

Your shell must execute the ```exit``` command where typing in ```exit``` quits the shell. 

### Turn in
* An autograder will be implemented on gradescope. Part 1 will be due 14-Feb 11:00 PM <3
* Submit all files needed to run your program, and a make file. The make file should build your entire project using ```make all```
* Your executable should be called ```361_shell```
* _Projects that fail to comply with the above will not be graded._ 

### Input
* ```<command>``` will be called using its absolute path. IE ls will be called as /bin/ls
* You can assume that command arguments will be separated by spaces. There will be no quotations.
