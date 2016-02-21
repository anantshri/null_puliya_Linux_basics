---
---
# SHELL SCRIPTING

## Linux Variables

* $$ = The PID number of the process executing the shell. 
* $? = Exit status variable. 
* $0 = The name of the command you used to call a program. 
* $1 = The first argument on the command line. 
* $2 = The second argument on the command line. 
* $n = The nth argument on the command line. 
* $* = All the arguments on the command line. 
* $# The number of command line arguments.

## Conditional Checks

__Test__

There is a function provided by bash called test which returns a true or false value depending on the result of the tested expression. Its syntax is: 

__test expression__

* -b file = True if the file exists and is block special file. 
* -c file = True if the file exists and is character special file. 
* -d file = True if the file exists and is a directory. 
* -e file = True if the file exists. 
* -f file = True if the file exists and is a regular file 
* -g file = True if the file exists and the set-group-id bit is set. 
* -k file = True if the files' "sticky" bit is set. 
* -L file = True if the file exists and is a symbolic link. 
* -p file = True if the file exists and is a named pipe. 
* -r file = True if the file exists and is readable. 
* -s file = True if the file exists and its size is greater than zero. 
* -s file = True if the file exists and is a socket. 
* -t fd = True if the file descriptor is opened on a terminal. 
* -u file = True if the file exists and its set-user-id bit is set. 
* -w file = True if the file exists and is writable. 
* -x file = True if the file exists and is executable. 
* -O file = True if the file exists and is owned by the effective user id. 
* -G file = True if the file exists and is owned by the effective group id. 
* file1 –nt file2 = True if file1 is newer, by modification date, than file2. 
* file1 ot file2 = True if file1 is older than file2. 
* file1 ef file2 = True if file1 and file2 have the same device and inode numbers. 
* -z string = True if the length of the string is 0. 
* -n string = True if the length of the string is non-zero. 
* string1 = string2 = True if the strings are equal. 
* string1 != string2 = True if the strings are not equal. 
* !expr = True if the expr evaluates to false. 
* expr1 –a expr2 = True if both expr1 and expr2 are true. 
* expr1 –o expr2 = True is either expr1 or expr2 is true.

Example

<pre>
test -b file
<\pre>
this will return true if file exists and is block special file

__Test shorthand__
most of the shell scripts will be using short hand version of test command as shown below

<pre>
[ -b file ]
<\pre>
note a blank space at both sides of brackets. this gap is important and is required.


## Iteration, control and if statements


### if

Used to execute one or more statements on a condition. 

An example: 
<pre>
if [ ! -d /mnt ]		
then
   mkdir /mnt
fi
<\pre>

### case

Used to execute specific commands based on the value of a variable.

An example: 

<pre>
case $NUM of
1)
   echo The number is 1
   ;;
2)
   echo The number is 2
   ;;
*)
   echo The number is not 1 or 2
   ;;
esac
<\pre>


### for 

Used to loop for all cases of a condition.

Example: Here we have used 2 things 

1. for loop 
2. variable expansion {1..10} expands to 1 2 3 4 5 6 7 8 9 10

So in short below for loop will print 1 to 10

<pre>
for i in {1..10}; do
   echo $i
done
<\pre>

### until 

Cycles through a loop until some condition is met. The syntax for the command is shown below: 

<pre>
until [ expression ]
do
   statements
done
<\pre>

### while 
Cycles through a loop while some condition is met. The below example will cycle through a loop forever: 

<pre>
while [ 1 ]
do
   statement(s)
done
<\pre>
