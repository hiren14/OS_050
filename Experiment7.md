<h1 align="center" style="margin-top: 0px;"> Experiment 7 </h1> 

# Aim:-   Write a menu driven shell script which will
- print the following menu and execute the given task.
-   a. Display calendar of current month
-   b. Display today’s date and time
-   c. Display usernames those are currently logged in the system
-   d. Display your name at given x, y
# code :- 

```bash

i=0
while [ $i != 6 ]
do
echo "Menu
1. Display calender of current Month
2. Display today's date and time
3. Display usernames of those who are currently logged in the ststem
4. Display your name at given x, y position
5. Display Terminal Number
6. Exit
Choose your option and enter corresponding value"
 
        read i
        case "$i" in
                1) calender="$(cal)"
                        echo "Here is your Calender "
                        echo "$calender"
                        ;;
                2) current="$(date)"
                        echo "Current Date and Time is " "$current"
                        ;;
                3) username="$(whoami)"
                        echo "Currently logged in users : "
                        echo $username
                        ;;
                4)                         
                        ;;
                5) 
                        ;;
esac
done

```
<hr />

# Output

![p1a](https://hiren14.github.io/OS_050/output/exp7.png)
