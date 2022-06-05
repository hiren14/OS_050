<h1 align="center" style="margin-top: 0px;"> Experiment 2  </h1> 

# Aim:-  Write a shell script to generate marksheet of a student. Take 3 subjects, calculate and display total marks, percentage and Class obtained by the student.

```bash
#!/bin/sh

echo "enter maths marks"
read maths
echo "enter english marks"
read english
echo "enter science marks"
read science

sum=`expr $maths + $english + $science`
echo "sum of three subject are:" $sum
per=`expr $sum / 3`
echo "percentage is:" $per
if(($per >= 60))
then
        echo "you got distinction"
elif(($per <= 33))
then
        echo "you failed"
else
        echo "you passed"
fi
```
# Output
<hr />


![p1a](https://hiren14.github.io/OS_050/output/exp2.png)
