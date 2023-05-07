---
name: Reyker Ventura 
course: cis106
semester: spring 2023
---

# Question 1

## Awk
* Description:
      * Awk is a scripting language used for processing and displaying text. Awk can work with a text file or from standard output.
 * Formula: 
 * 'awk + options + {awk command} + file'
 * 'command output' | 'awk + options + {awk command}'

* Examples:
 * how to print the first field of a file:
      * awk -f':' '{print $1}' /etc/passwd'
 * how to start printing from a different line 
     * 'awk 'NR > 3 {print}' /etc/passwd'
* how to change a field to upper case:
    * awk -F: '{print toupper($1)}' 

## cat
* Description: the cat is used for displaying the content of a file. cat is short for concatenate which is its command intended use.
* Formula:
      * cat + option +file(s) to display
  
  * Example: Display the content of a file located in the pwd
      * cat todo.lst
* Display the content of a file using absolute path
      * cat ~/Documents/todo.lst 


## cp
## cut
* Description: The cut command is used to extract a specific section of each line of a file and display it to the screen.
* formula: cut + file(s)

* Example: Display a list of all the users in your system:
      * cut -d ';' -f1 /etc/passwd
* Display a list of all the users in your system with their login shell
      * cut -d ';' -f1,7 /etc/passwd




## grep
* Description: Grep is used to search text in given file. Grep work line by basis( it matches the search criteria in a line by line basis).
  * Formula:
      * grep + option + search criteria + file(s)

*Example:
Search any line that contains the word "dracula" in the given file:
      *   grep 'dracula' ~/Documents/dracula.txt



## head
* Description:
    *   The head command displays the top N number of lines of a given file. By default, it prints the first 10 lines. If more than one file name is provided then data from each file is preceded by its file name.
  
  * Formula:
      * 'head + option + file(s)
  
* Example: Display the first 10 lines of a file
      * head ~/Documents/Book/dracula.txt
* Display the first 5 lines of a file:
      * head -5 lines of a file   




## ls
## man
## mkdir
## mv
## tac
* Description:
  * The cat command is used for displaying the content of a file. Cat is short for concatenate which its command intended use.
  * Formula:
    * 'tac + option + file(s) to display
  
* Example: Display the content of a file located in the pwd:
    * tac todo.md
* Display the content of a file using absolute path:
    * tac ~/Documents/todo.md



## tail
* Description:
  * the tail command displays the last N number of lines of a given file. By default, it prints the last 10 lines. If more than one file name is provided then data from each file is preceded by is file name.
  
  * Formula: 
      * 'tail ~/Documents/Book/dracula.txt

* Example: Display the last 10 lines of a file:
      * tail ~/Documents/Book/dracula.txt
* Display the last 5 lines of a file:
      *  tail -5 ~/Documents/book/dracula.txt 


## touch
## tr
## tree