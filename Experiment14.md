<h1 align="center" style="margin-top: 0px;"> Experiment 14 </h1> 

#   Aim:-   Write an awk program using function, which convert each word in a given text into capital. 
#   code :- 

```bash

read -p "Enter a lowercase String : " string
echo "Resultant Upercase string is : "
echo "$string" | awk '{print toupper($0)}'

```
<hr />

#   Output


![p1a](https://hiren14.github.io/OS_050/output/exp14.png)
