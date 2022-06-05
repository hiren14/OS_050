<h1 align="center" style="margin-top: 0px;"> Experiment 11 </h1> 

#   Aim:-   Shell programming using filters (including grep,egrep, fgrep)
#   code :- 
#   1. cat: Displays the text of the file line by line.

###  Syntax

```bash
  cat [path]
```
<br />
<br />
<hr />

#   2. head: Displays the first n lines of the specified text files. If the number of lines is not specified then by default prints first 10 lines.
Syntax

```bash
	 head [-number_of_lines_to_print] [path]
```

#   3. tail: It works the same way as head, but in reverse order. It returns the lines from bottom to up

```bash
	tail [-number_of_lines_to_print] [path] 
    
```
<br />

#   4. sort: sorts the lines alphabetically by default but we can customize the way of sorting.

```bash
	sort [-options] [path]
```
<br />

#   5. uniq: removes duplicate lines. it has a limitations that it can only remove continuous duplicate lines.


```bash
	uniq [options] [path]
```
<br/>

#  6. wc: It gives the number of lines, words and characters in the data.

```bash
	 wc [-options] [path]
```

-   wc gives 4 outputs as
-   	number of lines
-   	Number of words
-   	Number of characters
-   	path


#   7   grep: grep is used to search a particular information from a text file.


```bash
	grep [options] pattern [path]
```
#   8. tac: It is just reverse of cat command. It prints from bottom to top.

```bash
	tac [path]
```

# 9. Sed: It stands for stream editor. It allows us to apply search and replace operation on our data effectively.

```bash
	sed [path]
```
# 10. nl: It is used to number the lines of our text data.

```bash
	nl [-options] [path] 
```
