<h1 align="center" style="margin-top: 0px;"> Experiment 13 </h1> 

#   Aim:-   Write a shell script which will generate first n fibonnacci numbers like: 1, 1, 2, 3, 5, 13, …

#   code :- 

```bash

echo "Date validator"
#Initializing values of date, month and year
dd=0
mm=0
yy=0
 
#initializing no of days in a month
days=0
 
read -p "Enter day (dd) : " dd
read -p "Enter Month (mm) : " mm
read -p "Enter Year (yyyy) : " yy
 
#checking for invalid month
if [ $mm -le 0 -o $mm -gt 12 ]
then
        echo "$mm is invalid month. "
        exit 1
fi
 
#finding out no. of days in a month
case $mm in
        1 | 3 | 5 | 7 | 8 | 10 | 12)
                days=31
                ;;
        2)
                days=28
                ;;
        4 | 6 | 9 | 11)
                days=30
                ;;
        *)
                days=-1
                ;;
esac
 
#checking for leap year
if [ $mm -eq 2 ]
then
        a=`expr $yy % 4`
        b=`expr $yy % 100`
        c=`expr $yy % 400`
 
        if [ $a -eq 0 -a $b -ne 0 -o $c -eq 0 ]
        then
                days=29
        else
                break
        fi
fi
 
if [ $dd -le 0 -o $dd -gt $days ]
then
        echo "$dd day is invalid "
        exit 3
fi
 
#No error means date is valid
echo "$dd/$mm/$yy is a Valid Date"

```
<hr />

# Output


![p1a](https://hiren14.github.io/OS_050/output/exp13.png)
