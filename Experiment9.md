<h1 align="center" style="margin-top: 0px;"> Experiment 9 </h1> 

# Aim:-   Write a shell script to display all executable files, directories and zero sized files from current directory.
# code :- 
```bash

echo "Executable files"
files="$(find lab_solutions -executable -type f)"
echo "$files"
echo
echo "List of Directories"
dir="$(ls -d */)"
echo "$dir"
echo
echo "List of zero sized files"
zero="$(find -size 0)"
echo "$zero"

```
<hr />

# Output :- 

![p1a](https://hiren14.github.io/OS_050/output/exp9.png)
