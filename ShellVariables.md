# Shell Variables

## Printing Variables
The echo command, which outputs the arguments passed to it, also displays the values of variables when they're preceded by a $. In this challenge, I needed to display the FLAG variable, so I used the command echo $FLAG.

```
Flag: pwn.college{8kRrfV2AaLKq0UXnP7oftizrzBd.dJDN4QDLyYTN0czW}
```
## 


## Setting Variables
 Variables can be assigned values using the = operator, ensuring there are no spaces between the variable name and the equal sign. Unlike when accessing the value, the $ is not required during assignment. In this case, I needed to assign the value COLLEGE to PWN, so I used the command PWN=COLLEGE.
```
Flag: pwn.college{cvb-1SDNLL3mN49dY8DthOD5Mgs.dNDN4QDLyYTN0czW}
```
## 



## Multi-Word Variables
Spaces in a variable's name or value can lead the shell to mistakenly treat the word following the space as a separate command. To avoid this, you can enclose the variable value in quotes. For instance, to assign PWN the value COLLEGE YEAH, I used the command PWN="COLLEGE YEAH".
```
Flag:  pwn.college{sRoPqLqU7S5bBaxftS-eJUf9K7V.dVDN4QDLyYTN0czW}
```
##


## Exporting Variables
When assigning variables, they are only accessible within the current shell process and can't be inherited by a child process, such as one started using sh. First, to export the value COLLEGE to the variable PWN, I ran export PWN=COLLEGE. Then, to assign PWN to COLLEGE without exporting it, I used COLLEGE=PWN. Finally, to verify if only PWN was exported, I launched a new shell using sh and executed /challenge/run to retrieve the flag.
```
Flag: pwn.college{sMuLtG_gQRIEw-FZxzlmLJkTduw.dZDN4QDLyYTN0czW}
```
##


## Printing Exported Variables

Just ran the env command and retrieved the flag.
```
Flag:  pwn.college{kb7L0xTGQKlR1IFEubIjPG8-ZRg.ddDN4QDLyYTN0czW}
```
##


## Storing Command Output

Command substitution allows you to capture the output of a command and store it in a variable. In this, I stored the output of /challenge/run into PWN by running PWN=$(/challenge/run), and then displayed it using echo "$PWN".
```
Flag: pwn.college{8v7xrrWdAOVzjVJEJ-V42CBUd8j.dhDN4QDLyYTN0czW}
```
## 


## Reading Input

The read command is used to capture input from the user. In this, I needed to assign the value COLLEGE to the PWN variable using read. I accomplished this by running read -p "Input: " PWN, then entering COLLEGE as the input, which gave me the flag.
```
Flag: pwn.college{kdYZR8CKqEGfjt_7E59J-NEDXZP.dhzN1QDL0QjN0czW}
```
##


## Reading Files

To read the contents of /challenge/read_me into the variable PWN, I used the command read PWN < /challenge/read_me.
```
Flag: pwn.college{UNRzREWYuhxdwzY7C2-jWcTWyew.dlDN4QDLyYTN0czW}
```
##