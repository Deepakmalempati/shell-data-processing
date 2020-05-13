# Module 1 - Shell Data Processing

1. curl command used to get data - ```curl "https://en.wikipedia.org/wiki/COVID-19_pandemic"```
2. command for most common words and sorted - ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr```

## My notes

In this module i have worked on a simple bigdata process to find out words that apprear most frequently in a webpage.

### Step 1 - Retriving data from URL
- to retrive the data from url use following command  
``` curl "url"```
- To copy the retrived text to a file  
``` curl "url -O filename.txt```
### Step2 - Working with the data
- below command is used to replace space with a character  
``` tr ' ' '\12' < data.txt```
- below bash command is used to sort the input  
``` tr ' ' '\12' < data.txt | sort```
- below command is used to find character count from the sorted data  
``` tr ' ' '\12' < data.txt | sort | uniq -c ```
- sort the data with unique characters using nr flag.  
``` Hint: tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr ```
- To move the result to a specific file  
``` tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt```
- up arrow is used to see the bash commands that are executed before
- ```-n``` is used to sort the numerical value according to String numerical 
- ```-r``` is used for reversing the result from comparision

### Important Bash Commands
- Bash redirect is used for redirecting contents of the directory into a file.  
Example: ```ls > data.txt```
- Bash redirect and append is used to append new data instead of overwriting the data  
Example: ```ls >> data.txt```
- ```ls``` is used to show list of contents in the directory
- ```cat``` command is used for displaying contents
- to copy something in Bash use CTRL+SHIFT+C
