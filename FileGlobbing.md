# FILE GLOBBING
## CHALLENGE 1: matching with *
This wasnt new information with me we have used this type of wild character matching in sql so it was easy for me. Foud the flag easily.
```
flag obtained: pwn.college{4Zt5DmrTF1brx6Bq50b9TjUg1Zj.dFjM4QDLyYTN0czW}
```
##


## CHALLENGE 2: matching with ?
Again similar to sql but as far as i rememeber in sql "_" is used to match single character. Used this to replace c and l and ran the program. Curious as to how pwn.college checks if we have used wildcard character or not.
``` 
flag obtained: pwn.college{kFrdMNPFd9EsdGeihWl8xY35xAi.dJjM4QDLyYTN0czW}
```
##


## CHALLENGE 3: matching with []
This was new to me but seemed easy to use and was. Its nice and easy how we can obtain multiple files at once using one command. I was easily able to obtain the flag.
```
flag obtained: pwn.college{8UsCOaNp81iluvt5vDODdgTQ4qs.dNjM4QDLyYTN0czW}
```
##


## CHALLENGE 4: matching paths with []
Nice how we can use [] to run programs as well and provide arguments. This challenge was a little tricky as we had to mention the absolute path to the files as well as argument. Took me sometime but I was able to do it.
```
flag obtained: pwn.college{UcgZigxmXC16cgLzNjYs-OpIEKO.dRjM4QDLyYTN0czW}
```
##


## CHALLENGE 5: mixing globs
Mixed the globs and used [cep]* to find the particular files and obtained the flag. Took sometime to find the relationship between the 3 files but there wasnt any other relation. Kind of wasted my time on this a little.
```
flag obtained: pwn.college{QzTXiwZAkk0D1sTCvxZatEs-YO5.dVjM4QDLyYTN0czW}
```
##


## CHALLENGE 6: eclusionary glob
Learnt the usage of the ^ command. Kind of like the != command in coding languages. Found the flag with ease
```
flag obtained: pwn.college{M7hE6uhyHW-p-RJ_HUFLZMIB3IC.dZjM4QDLyYTN0czW}
```
##