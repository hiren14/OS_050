<h1 align="center" style="margin-top: 0px;"> Experiment 6 </h1> 

# Aim:-   Write a shell script which will generate first n fibonnacci numbers like: 1, 1, 2, 3, 5, 13, …
<br />

#       code :- 

```bash


#!/bin/sh

echo "enter how many number you want in series"
read n
echo "first $n fibonnaci numbers are:"
a=1
b=1
echo "$a"
echo "$b"

for((i=0;i<n-2;i++))
do
        c=$(( $a + $b))
        echo "$c"
        a=$b
        b=$c

done
```
<hr />

# Output

![p1a](https://hiren14.github.io/OS_050/output/exp6.png)
