# PRACTICING PIPING
## CHALLENGE 1: redirecting output
learnt what redirecting is and what the > command does. Used echo PWN > COLLEGE to reidrect the outpur of the command which will be pWN to the file college and obtained the flag.
```
flag obtained: pwn.college{kCNYZ5w6zHvUeTfA4cwN7Z25vc5.dRjN1QDLyYTN0czW}

```
##


## CHALLENGE 2: redirecting more output
used the command > to redirect the output to the file. Then read the file and obtained the flag.
```
flag obtained: pwn.college{s_xXiBJDyPZsFlvVut3hqJxN7_b.dVjN1QDLyYTN0czW}
```
##


## CHALLENGE 3: appending output
learnt that >> is used to append to a file while > truncates the file. Similar to opening a txt file in append and w mode. Appending to the file and got the. Nice how theyve split the flag in 2 parts to ensure us appending.
```
flag obtained: pwn.college{gFC2vW6Eyjp3RmVNXnV6QA8cNVz.ddDM5QDLyYTN0czW}
```
##


## CHALLENGE 4: redirecting errors
Learnt that you can redirect errors, input and output. This challenge I did what was told which was easy enough and obtained the flag. New information that we can redirect errors and input as weel seems cool.
read the file and got the flag after redirecting error and output.
```
flag obtained:  pwn.college{IyeAEUexpGaKXGaNa1ILRzONTTS.ddjN1QDLyYTN0czW}
```
## 


## CHALLENGE 5: redirecting input
Learnt that we can redirect input as well. In this we write into the file pwn using redirection. Then redirect that as input to /challenge/run and then get the output and the flag.
```
flag obtained: pwn.college{Ye6QSHd2kDWwWAkHmPlktj7MBzI.dBzN1QDLyYTN0czW}
```
##


## CHALLENGE 6: grepping stored results
Redirected the poutput of the program to a tect file and grepped the flag from there. Like previous questions.
```
flag obtained: pwn.college{Yh4YttyVJpFtR-M5sljoyL1xZAB.dhTM4QDLyYTN0czW}
```
##


## CHALLENGE 7: grepping live output
Learnt about the pipe command which seems like a command to use to run simultaneous commands. seems like a very useful command. Used this command to run the program and grep the flag at the same time in one command.
```
flag obtained: pwn.college{UtwKe5c4MskBHsZqImr4G4O2yEI.dlTM4QDLyYTN0czW}
```
##


## CHALLENGE 8: grepping errors
In this challenge we redirected error the output of the program and converted it to standard input as the pipe command only takes standard output as a value, so we used the >& command and converted the erros output to standard input and then grepped the flag.
```
flag obtained: pwn.college{UtwKe5c4MskBHsZqImr4G4O2yEI.dlTM4QDLyYTN0czW}
``` 
##


## CHALLENGE 9: duplicating piped data with tee
Learnt the usage of the tee command then used the tee command and copies the contents of /challenge/pwn to /challenge/college then found the seceret value and used it to proeprly run the /challenge/pwn command and piped /challenge/college and found the flag.
```
flag obtained: pwn.college{0cUrxA4IlWbiTnz1J3IaDDKh-Ya.dFjM5QDLyYTN0czW}
```
##


## CHALLENGE 10: writing to multiple programs
In this challenge i took the output of /challenge/hack and passed it as input for for the file /challenge/the and used it as input for /challenge/planet as well using the pipe and tee commands. Took a while to read snd understand this challenge but it taught me a lot of things.
```
flag obtained: pwn.college{0G7lD7Um2zSjD-7jgVB5AHc7s7u.dBDO0UDLyYTN0czW}
```
##


## CHALLENGE 11: split-pipping stderr and stdout
In this we used did a similar thing to the previous challenge and connected the standard output of /challenge/hack to /challenge/input and all the errors of /challenge/hack to /challenge/the using substituion. These last 2 questions were very tricky and had me stumped for a while.
```
flag obtained: pwn.college{ogmB4eJMSeFPPMRPRTswwO6xy7g.dFDNwYDLyYTN0czW}
```
##

