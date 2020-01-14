# Welcome to Introduction to UNIX 

  Today I am going to tell you some basic things about UNIX operating system whatever I learned from a short tutorial on introduction to UNIX for beginners.
  
  UNIX is an operating system there was first developed in the 1960s and has been under constant development ever since. By operating system, we mean the suite of programs which make the computer work. It is a stable, multi-user, multi-tasking system for servers, desktops, and laptops. 
  
  UNIX also has a graphical user interface like Microsoft windows but we should know UNIX commands to carry out the operations which can not be done by graphical programs or when there are no graphical interactions like telnet session.

# Types of UNIX :
  There are so many distros of UNIX are available. The most popular varieties of UNIX are Sun Solaris, GNU/Linux, and macOS X. 

# UNIX OS:
  UNIX is made up of shell, kernel, and programs.
  
 **Kernel**:- It is called the heart of the operating systems. It allocates time and memory for the processes.\
 **Shell**:-  It is the interface between the kernel and user. It takes the commands from the user, interprets them and gives it to the kernel for the execution.
  
  In UNIX everything is considered as either file or process.
  Process means the program in the running state.
  The file is the collection of the data.
  There are two types of files as normal files and directories.
  
  All the files are grouped together in the directory structure. The file-system is arranged in a hierarchical structure, like an inverted tree. The top of the hierarchy is traditionally called root (written as a slash / ).
  
  There terminal in UNIX operating system where we can run our commands.
  
# Basic UNIX Commands in Short
  **ls dir**:-
    This command is used to display the name of all files and folders from the specified directory or subdirectory.
There are various options are available with the ls. You can explore them by using the internet. ~ denotes root directory.

**mkdir dir**:-
    This command is used to create a new directory on a specified path. if you do not provide any path then the directory is created at the current directory.
    
**cd path**:-
    This command is used to change the directory. When we use with the cd command it denotes current directory and when we use .. then it denotes the parent directory.
    
**pwd**:-
    This command gives the path of the present working directory.
    
**cp src dest**:-
    This command is used to copy the files either in the same directory or in the specified directory.
    
**mv src dest**:-
    This command is used to move files. If we move the file in the same directory with a different name then it is working as the renaming of file.
    
**rm file_name**:-
    This command is used for removing the specified file.
    
**rmdir dir_name**:-
    This command is used for removing the directories.
    
**cat file1 file2**:-
    cat stands for concatenate. The command cat can be used to display the contents of a file on the screen.
    
**less file**:-
    The command less writes the contents of a file onto the screen a page at a time.
    
**head file**:-
    The head command writes the first ten lines of a file to the screen. 

 **tail  file**:-
     Display the last few lines of a file.
 
 **grep 'keyword' file** :-
    search a file for keywords. 

 **wc file** 
     count number of lines/words/characters in file

# Redirection
**command > file**:-
    Here > is used to write the output of the command as input to the file.

**command > file**:- 
    Here >> is used to append and write the output of the command as input to the file.

**command < file**:-
    Redirect the input to command from the file.

# Pipes: 
**command1 | command2**:-
    It gives the output of the  command1 as input for command2.

**sort**:-
    This command is used to display the given data in sorted order.

**who**:- 
    List the users who currently logged in the system.

# Wildcards:##
**The * wildcard**: -
    The character * is called a wildcard, and will match against one or more character(s) in a file (or directory) name.

**The * wildcard**:
    The character ? will match exactly one character.

# Getting help:
**man command**:
    This will show you the manual page of the command. This page demonstrates the use of the specified command.

**whatis command**:
    This will give a description in one line of the specified command.

**apropos keyword**:
   When you don't know the exact command then you can use the apropos command with the related keyword which will show all related commands with that keyword.
   
**File Permissions:**
    In UNIX Each file (and directory) has associated access rights/permissions with it. 
        *-rwxrw-r-- 1 admin1 admin1   64 Jan 13 12:20 newlist* 
    As you can see above, r stands for read permission,w stands for write permission and x stands for execution permission.
    
**Access rights/permissions on files:**
    **r** : It indicates read permission, that is the presence or absence of permission to read and copy the file
    **w** : indicates write permission, that is the permission (or otherwise) to change a file
    **x** : indicates execution permission, that is the permission to execute a file, where appropriate

**Access rights/permissions on directories:**
    **r** : allows users to list files in the directory;
    **w** : means that users may delete files from the directory or move files into it;
    **x** : means the right to access files in the directory. This implies that you may read files in the directory provided you have read permission on the individual files.
# Changing Access Rights/Permissions
   By using *chmod* command we can change the permissions of the files or directories.
   
| Symbol  | Meaning   |
|:-:|:-:|
| u  | user  |
|  g |  group |
|  o |  other |
| a  | all  |
| r  | read  |
| w  | write  |
|  x | execute  |
|  + | add permissions  |
| -  | remove permissions  |

examples:-
    __*chmod go-rwx biglist*__
        This command will remove read, write and execute permission of the file for group and others.
    __*chmod a+rw biglist*__
    This command will add read and write permissions to all.
# Processes and Jobs :
Executing program is called the process and each process has unique PID(process ID) by which it is uniquely identified.
