# Module 1 - Shell Data Processing

In this module i have worked on a simple bigdata process to find out words that apprear most frequently in a webpage.

### Step 1 - Retriving data from URL
- to retrive the data from url use following command
``` curl "url"```
- To copy the retrived text to a file
``` curl "url -O filename.txt```
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
