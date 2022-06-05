<h1 align="center" style="margin-top: 0px;"> Experiment 2 </h1> 

# Aim:-  Write a shell script to display multiplication table of given number.
## code :- 
```bash

#!/bin/sh

echo "enter number for multiplication table:"
read n

for((i=1;i<=10;i++))
do
        echo " $n*$i=$((n*i))"
done
```
<hr />

# Output


![p1a](https://hiren14.github.io/OS_050/output/exp3.png)
