# Proccess And Jobs

## Listing Processes

Used ps aux and then ran the required command.
```
Flag: pwn.college{gccYZs0MbGT4fgVw-eMYEUZcYLm.dFTM2QDLyYTN0czW}
```
##


## Killing processes

To terminate /challenge/dont_run so that /challenge/run could execute, I first found its PID using ps -e | grep /challenge/dont_run, which returned 73. I then executed kill 73 to stop the process, followed by running /challenge/run to retrieve the flag.
```
Flag: pwn.college{8Hct7sqnV4MmWESJLv81op9cMIV.dFzNyUDLyYTN0czW}
```
##


## Interrupting processes

Ran challenge/run and used ctrl+c to interrupt it.
```
Flag:  pwn.college{UFaa3Y-uQq2xIv8h38UwQJQYtqm.dJzNyUDLyYTN0czW}
```
##


## Suspending Processes

Ran challenge/run, then ctrl+z then ran the command again after which I retrieved the flag.
```
Flag: pwn.college{kZH9lEaUmTDDiEVHhdecjq_SJ-v.dNzNyUDLyYTN0czW}
```
##


## Resuming Processes

Ran challenge/run, then ctrl+z then ran the command fg /challenge/run after which I retrieved the flag.
```
Flag: pwn.college{ADmgK0qGx37Y-apT6F8J9h0KewQ.dJTM2QDLyYTN0czW}
```
##


## Backgrounding Processes

Similar to before, I used bg /challenge/run, after which I ran /challenge/run again.
```
Flag: pwn.college{QiqaRpFCZc8nXri14vwNaY91zZA.dVTN0UDLyYTN0czW}
```
##


## Foregrounding Processes

This challenge involved first suspending /challenge/run using Ctrl-Z, then resuming it in the background with bg /challenge/run, and finally bringing it back to the foreground using fg /challenge/run.
```
Flag: pwn.college{kKkEdEgMMLllgJ4ZO93DzBLwAzt.dZTN0UDLyYTN0czW}
```
##


## Starting background processes

To run /challenge/run in the background and retrieve the flag, I simply executed /challenge/run &.
```
FLag: pwn.college{IfBTZcugkhrLi8kL9S8g0KsNs7S.ddTN0UDLyYTN0czW}
```
##


## Process Exit Codes

To obtain the exit code of /challenge/get-code, I executed it, and it terminated with an error code. I then ran echo $?, which returned 236. Subsequently, I passed this code as an argument to /challenge/submit-code 236 and successfully retrieved the flag.
```
Flag: pwn.college{4VCyJbCkzt5AnPkEpphF4EadIKL.dhTN0UDLyYTN0czW}
```
##