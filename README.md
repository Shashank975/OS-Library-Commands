# OS-Library-Commands
OS library / Operating System library is used to automate the commands that we used to type in our terminals in order to complete a task like creating a folder, deleting a folder etc.

OS Basics  

import os : used to import the os library

os.getcwd : used to get the current working directory(cwd).

os.chdir(“directory_name”) : To go inside a folder.

os.chdir(“..”) : To go back to the previous directory.

os.mkdir(“file_name”) : To create a directory in the cwd.

os.mkdirs(“filename/filename1/filename2”): Used to create directories within directories.

os.remove(“File_Name”): can be used to remove a folder but if folder is empty if it contains anything it can’t be used.

os.rmdir(“parent_name/sub_directory_name”):

Example os.rmdir(“Test/Test1”) then os.rmdir(“Test”)

os.rename(‘old_file_name’,’new_file_name’) : used to rename a file

os.getsize(“folder_name”) : gives size of folder in kbs.

 

 

Note in order to use CLI commands in jupyter we should use ! mark before the command like   !touch file.txt         !ls    !pwd etc

 

To see all the sub-directories contained in a directory

Let’s say we have a folder Imgs and want to check all the sub-directories contained in the directory Imgs we can automate this by:

for i in os.listdir('Imgs'):

    if i != '.DS_Store':  ##System

        print(i)

This code can be used to print all the sub-directories present inside the directory Imgs.

 

To check If a path exists or not:

os.path.exists(“path”): Example os.path.exists(“Imgs/Test1”) this will return a Boolean result.

To check if a folder exists if it doesn’t exists then creating the folder.
