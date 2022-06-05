<h1 align="center" style="margin-top: 0px;"> Experiment 5 </h1> 

# Aim:-  Write a shell script which will accept a number b and display first n prime numbers as output.
# code :- 
#!/bin/sh
```bash

echo "enter number"
read n
echo "prime numbers up to $n are:"
m=2
while [ $m -le $n ]
do
        i=2
        flag=0
        while [ $i -le `expr $m / 2` ]
        do
                if [ `expr $m % $i` -eq 0 ]
                then
                        flag=1
                        break
                fi
                i=`expr $i + 1`
        done
        if [ $flag -eq 0 ]
        then
                echo $m
        fi
        m=`expr $m + 1`
done

```
<hr />

#       Output

![p1a](https://hiren14.github.io/OS_050/output/exp5.png)
