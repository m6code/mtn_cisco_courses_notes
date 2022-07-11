# NDG Linux Unhatched Course
### Info
* Duration : 8 Hours

## Notes
* Technical skills to analyze, process, protect, and transmit data are therefore also in high demand. Learning Linux can help you on the journey towards acquiring these skills

* Example of IT Professions includes Network Engineeering, Cybersecurity, Developing/programming, Data Analysis

### Section 2 - Basic Command Syntax
* A command is a software program that when executed on the CLI (command line interface), performs an action on the computer.
* Every part of the command is normally case-sensitive
* An argument can be used to specify something for the command to act upon.
* Options can be used to alter the behavior of a command.
* Basic command syntax is `command [options…] [arguments…]`.
    * for example `ls -l Documents`. here ls = command; -l is an option, and Documents is the argument

* Multipe Options can be given in any other and it would work the same for example 
    ```
    ls -l -r
    ls -rl 
    ls -lr 
    ``` 
    would all do the same thing. 

### Section 3 - Printing Working Directory
* In order to discover where you are currently located within the filesystem, the pwd command can be used. The pwd command prints the working directory, your current location within the filesystem:
### Section 4 - Changing Directories
* Files are used to store data such as text, graphics and programs. Directories are a type of file used to store other files–they provide a hierarchical organizational structure. 
* To navigate the filesystem structure, use the cd (change directory) command to change directories. basic structure `cd [options] [path]`
* the top directory of the linux system (root directory)is represented by the `/` (forward-slash) character while the home (user) directory is represented by `~` (tilda) character
* There are two types of parts 
    1. Absolute paths : allows you to specify the exact location of a directory. It always starts at the root directory, therefore it always begins with the / character. e.g `cd /home/user/Desktop` is an absolute path.
    2. Relative paths : gives direction to afile relative to your current location in the filesystem. They start with the name of a directory and not with the / character.e.g `cd Documents`
* Regardless of which directory you are in, `..` always represents one directory higher relative to the current directory, sometimes referred to as the parent directory. 
* Regardless of which directory you are in, the `.` character always represents your current directory.

### Section 5 - Listing Files
* The ls command is used to list the contents of a directory. Basic syntax is `ls [OPTIONS] [FILE]`. By default, when the ls command is used with no options or arguments, it will list the files in the current directory.
* To learn the details about a file, such as the type of file, the permissions, ownerships or the timestamp, perform a long listing using the `-l ` option to the `ls `command. e.g `ls -l /var/log`
    ```
    -rw-r--r-- 1 root   root  18047 Dec 20  2017 alternatives.log       
            
    drwxr-x--- 2 root   adm    4096 Dec 20  2017 apache2 
    ```
    ![ls with -l argument details](./ndg_linux_unhatched/ls_command.png)

#### Sorting With ls
* `-t` option will sort the files by timestamp.
* `-S` option will sort the files by size.
* `-r` option will sort the files in reverse order.
