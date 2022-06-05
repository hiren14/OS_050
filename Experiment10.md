<h1 align="center" style="margin-top: 0px;"> Experiment 10</h1> 

# Aim:-   Write a shell script to check entered string is palindrome or not.
# code :- 
```bash
echo "Enter the string to check: "
read str
len=`echo $str | wc -c`
len=`expr $len - 1`
i=1
j=`expr $len / 2`
while test $i -le $j
do
        k=`echo $str | cut -c $i`
        l=`echo $str | cut -c $len`
        if test $k != $l
        then
                echo "String is not Palindrome"
                exit
        fi
        i=`expr $i + 1`
        len=`expr $len - 1`
done
echo "String is Palindrome"
```
<hr />

#       Output

![p1a](https://hiren14.github.io/OS_050/output/exp10.png)
