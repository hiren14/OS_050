<h1 align="center" style="margin-top: 0px;"> Experiment 8 </h1> 

# Aim:-   Write a shell script to read n numbers as
command arguments and sort them in
descending order. 
# code :-
```bash

read -p "Enter the number of values you want to sort "  n

for((i=0; i<$n; i++))
do
        read -p "Enter value of arr[$i]: " arr[$i]
done
#sorting code
for((i=0; i<$n; i++))
do
        for((j=0; j<n-i-1; j++))
        do
                if [ ${arr[j]} -lt ${arr[$((j+1))]} ]
                then
                        #swapping
                        temp=${arr[j]}
                        arr[$j]=${arr[$((j+1))]}
                        arr[$((j+1))]=$temp
                fi
        done
done
 
echo "Numbers sorted in descending order as"
echo ${arr[*]}

```
<hr />

# Output :- 

![p1a](https://hiren14.github.io/OS_050/output/exp8.png)
