# File Attributes
### chown command
Linux groups people on a system into three:  
Users  
Group  
Others  
The **chown** command changes the ownershp of a resource (file or directory)  
To check the current owner (user and group) of a file  
`ls darey`{{execute}}  
The third and fourth columns show the current owners (user and group) of the file.
The ownership for any file or directory can be changed as follows:  
`chown user:group darey`{{execute}}  
Where user designates the user you want to change the ownership to, and group designates the group (you can change this values as you wish)  
To recursively change ownerships of files in a directory, including the directory, use the **-R** flag  
`chown -R dare:developers pbl`  
  
### chmod Command
**chmod** is used to change the permissions on a file or directory. Permissions control who can use what actions on a resource.  
A file permission of READ ONLY prevents editing the file (or contents of the directory as the case may be).  
Linux file permission modes are as follows:  
READ - 4  
WRITE - 2  
EXECUTE - 1  
List the contents of your current directory  
`ls`{{execute}}  
The leftmost column shows the permissions associated with that file or directory.  
To set permissions on a resource with **chmod**, you add the modes above that you want to set. The modes comprise of the digits, first sets permissions for user, second for group and third digit sets permissions for others.  
  
`chmod 400 darey`{{execute}}  
This sets the permission for the current user to READ and the permissions for the GROUP - designated by the first 0 - to nothing (no permissions), same for the OTHERS (designated by the last 0).  
To allow read and write actions for user and group:  
`chmod 660 darey`{{execute}}