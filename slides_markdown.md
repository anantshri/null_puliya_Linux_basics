---
---
<!-- .slide: class="center" -->
# Linux Puliya

--

# Anant Shrivastava

* Information Security Consultant
* Admin - Dev - Security
* null + OWASP + G4H
* http://anantshri.info and @anantshri
* Trainer : Blackhat, RuxCon, NullCon, g0s, c0c0n
* Speaker : Nullcon, c0c0n, ClubHack, RootConf


| | |
|------------------|--------------|
| <center>&nbsp; [![Android Tamer](resources/images/androidtamer/android_tamer_icon50.png "Android Tamer")](https://androidtamer.com) &nbsp;</center>| <center> &nbsp; [![Code Vigilant](resources/images/codevigilant/logo50.png "Code Vigilant")](https://codevigilant.com) &nbsp;</center> |
| <center>Android Tamer</center> | <center>Code Vigilant</center> |
Notes:

In previous work life's been admin dev and security specialist.

--

# What are we covering

1. Understanding *nix
2. File System Basics
3. Understanding I/O
4. Basic Commands
5. How to Exit VIM
6. Shell Script basics
7. Automation

--

# NIX 

1. Family of OS ranging from Unix, Linux, *BSD (FreeBSD, OpenBSD etc)
2. Follow same standards in terms of file systems, directory layout etc

--
# Linux

1. Free as in free speech not free beer
2. Everyone can create there own Distro
3. Hanna Montanna Linux

![Hanna Montana](resources/images/linux/hml.jpg "Hanna Montana")

and more

--

# Linux Distributions

2. Various Linux Distributions
1. Debian Based (apt-get / dpkg) 
1. RedHat based (yum / rpm)
4. LTS or not

--

# File System Basics

1. Everything is a file
1. File System Layout
1. Standard File system layout
	2. / as highest level
	3. /etc for all configuration
	4. /home : users home folder

--
<center>
![File System Layout](resources/images/linux/fslayout.png "File System Layout")
</center>

--
# File System Types

* ext2
	* Maximum file size = 16 GB to 2 TB
	* File system size = 2 TB to 32 TB
* ext3
	1. Journaling (Linux Kernel 2.4.15)
	1. Maximum file size = 16 GB to 2 TB
	1. File system size = 2 TB to 32 TB
* ext4
	1. Starting from Linux Kernel 2.6.19 ext4
	1. Maximum file size = 16 GB to 16 TB
	1. File system size = 1 EB
		1. 1 EB = 1024 PB 
		1. 1 PB = 1024 TB 


--
# More File System Basic

1. File System Permissions

	-rwxrwxrwx

1. Suid bits

	-rwsrwxrwx

2. sgid bit

	-rwxrwsrwx

3. sticky bit

	-rwxrwxrwt

4. First bit can be l,c,b,d,-

Notes: 
We can do user group based permission checks around here

--

# Sudo

1. id 0 is omnipotent
1. its suggested not to use root access
1. So how do we do high privilege actions


<center>
![Sudo](resources/images/linux/sandwich.png "Sudo")
</center>

--

# Standard I/O

1. Input  (<)
1. Output (>)
1. Error  (2>)

--

# Useful commands


1. ls, cd, mkdir 
1. cut 
1. grep
1. sed
1. sort
1. uniq
1. xargs
1. find
1. tr
1. ps
1. screen
1. netstat -lntp
1. file
--

# Editor
1. Vim
2. Nano
3. EMACS

--

# Installing Softwares

1. Debian
apt-get install <package name>

1. Redhat
yum install <package name>

1. python
pip install <package>

1. ruby
gem install <package>

1. npm / nodejs
npm install <package>


--

# more useful commands

1. python -m SimpleHTTPServer Port
1. !!
1. cd ~
1. cd -
1. mtr
1. mount and format
1. setting environment Variables

--

# Crontab

1. Automate periodic execution

<pre>
* * * * * * CMD
| | | | | | 
| | | | | +-- Year              (range: 1900-3000)
| | | | +---- Day of the Week   (range: 1-7, 1 standing for Monday)
| | | +------ Month of the Year (range: 1-12)
| | +-------- Day of the Month  (range: 1-31)
| +---------- Hour              (range: 0-23)
+------------ Minute            (range: 0-59)
</pre>

--

# Configuring Services

## SSH

Configuration file : /etc/ssh/sshd_config


--

# Using SSH

1. SSH Authentication
	1. Password
	1. SSH Key
1. How to Configure SSH Login via Key
1. ~/.ssh/authorized_keys

--

# Shell Script basics

1. Shebang
2. $1 $2, $* $@ $0
3. read
4. echo
5. cat
6. Conditions
7. Loop
8. Expansion {}

--

# Writing custom scripts

1. Write a shell script to calculate simple interest
2. Write a shell script to check whether no is even or odd
3. Print prime numbers from 1 to 5000

--

# Overload commands

1. alias
1. Why alias and why not
1. find location add path before everything else and then overload

--
<!-- .slide: class="center" -->
# Example

--
<!-- .slide: class="center" -->
# Questions

--
<!-- .slide: class="center" -->
# Thank You
