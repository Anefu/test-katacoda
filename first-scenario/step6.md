# Locating files
### find Command
**find** is used to search for files. You could specify regex expressions and every file that matches that expression will be returned.  

`find . -name file1`{{execute}}  
  
Finds all the files whose file names start with **file** (e.g file1, file2, file-test, file.txt etc.)  
`find . -name 'file*'`{{execute}}  
  
The **-name** flag tells the command to search for specific name (file1 in this case). Notice we specified the path to search for the file after the **find** command as **.**.  
  
Search for files inside the pbl directory  
`find pbl -name 'file*'`{{execute}}