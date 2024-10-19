# Perceiving Permissions


## Changing File Ownership

To change the ownership of /flag to hacker, I executed chown hacker /flag, and then I read its contents using cat /flag.
```
Flag: pwn.college{Afb5O2yDODWT8Ip3y7F2PESm600.dVTN4QDLyYTN0czW}
```
##


## Groups and Files

In this case, to change the group ownership of the flag file as hacker, I ran chgrp hacker /flag and then used cat /flag to read the contents of the flag file.
```
Flag: pwn.college{oK4VWyDLbJAyfVlhibFaO9by501.dFzN4QDLyYTN0czW}
```
##


## Fun with Groups Names

I ran id to find the group. Then, I proceeded as before, running chgrp and cat.
```
Flag: pwn.college{s6vJRhJYVzQFb68KlVmqlPEMhDx.dhTM5QDLyYTN0czW}
```
##


## Changing Permissions

To make the flag readable, I added read permission for other users by executing chmod o+r /flag, and then I used cat /flag to read the contents of the flag.
```
Flag: pwn.college{EuhQByK0c1lutwpCN68Tg_vj1cj.dRzNyUDLyYTN0czW}
```
##


## Executable Files

To make /challenge/run executable, I had to add the executable permission to the user by using chmod u+x /challenge/run, and then I executed it.
```
Flag:  pwn.college{EEvOlKnVeynoCkBiGbwpD8TXFzS.dZzNwUDLyYTN0czW}
```
##


## Permission Tweaking Practice

This challenge involved changing the permissions of /challenge/pwn according to specific requirements, starting with running /challenge/run. For example, to add read permission for the user, remove execute permission from the group, and grant read and write permissions to others, I ran chmod u+r,g-x,o+rw /challenge/pwn.Then, I executed chmod u+r /flag to make it readable, followed by using cat /flag to read it.
```
Flag: pwn.college{4KWyeoOEqtoQrCfO7NRbKrXOW3M.dVzNyUDLyYTN0czW}
```
##


## The SUID Bit

In this, I ran chmod u+s /challenge/getroot and executed it which made it run as root. Then I ran cat /flag to get the flag.
```
Flag: pwn.college{4y7N6WDEW4OLSTDmTZnlluxNZHt.dNTM2QDL0QjN0czW}
```
##
