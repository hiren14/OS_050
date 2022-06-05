<h1 align="center" style="margin-top: 0px;"> Experiment 4 </h1> 

# Aim:-  Write a shell script to find factorial of given number n.

## code :- 
```bash

#!/bin/sh

echo "enter number for find factorial"
read n

fact=1
for((i=1;i<=n;i++))
do
        fact=$((fact*i))
done
echo "factorial of " $n "is:"$fact

```
<hr />

# Output
![p1a](https://hiren14.github.io/OS_050/output/exp4.png)
