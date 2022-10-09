# NDG Linux Essentials (https://www.netacad.com/courses/os-it/ndg-linux-essentials)
### Info
* Course Duration : 70 Hours

## Chapter 2 - Operating Systems
* Search more on common OS for firewalls
* The generic term operating system is used to describe whatever software is booted and run on that device.
* The 3 Major OSes are Windows, Apple macOS, and Linux. Of these 3 OSes only Windows is unique in its underlying code. Both Apple's macOS and Linux are UNIX based.
* When a software release has many new features that haven’t been tested, it’s typically referred to as *beta*. After being tested in the field, its designation changes to *stable*
* Some distributions offer stable, testing, and unstable releases.
* The Debian distribution warns users about the pitfalls of using the “sid” (unstable) release
* Linux can be used in one of two ways: graphical (GUI) and non-graphical (CLI).
* The CLI environment is provided by an application on the computer known as a terminal.
* The terminal accepts what the user types and passes to a shell. 
* The shell interprets what the user has typed into instructions that can be executed by the operating system.
* the `w` command shows who is logged in.

### 2.4.1 Linux Distributions
**Red Hat**: (Fedora, CentOS, Scientific Linux)
* RPM - Red Hat Package Manager.
* RHEL - Red Hat Enterprise Linux.

**SUSE**: (OpenSUSE)

**Debian**: (Ubuntu, Linux Mint)

**Android**: 

**Raspbian**:

**Linux History**
* ![Linux History Map](./ndg_linux_essentials/LEv2_2_3.png)

### 2.4.2 Embedded Systems
* *embedded systems*  are designed to do a specific task on hardware optimized for only that purpose. 
* These systems encompass a tremendous diversity of devices that are used today, from cell phones to smart TVs and appliances, to remote monitoring systems for pipelines and factories.

## Chapter 3 - Working in Linux
### 3.1.1 - The Command Line Interface (CLI) 
* The command line interface (CLI) is a simple text input system for entering anything from single-word commands to complicated scripts.
### 3.2 Applications
The kernel of the operating system is like an air traffic controller at an airport, and the applications are the airplanes under its control. The kernel decides which program gets which blocks of memory, it starts and kills applications, and it handles displaying text or graphics on a monitor
* Applications make requests to the kernel and in return receive resources, such as memory, CPU, and disk space
* The kernel also abstracts some complicated details away from the application. For example, the application doesn’t know if a block of disk storage is on a solid-state drive, a spinning metal hard disk, or even a network file share
* A process is just one task that is loaded and tracked by the kernel. An application may even need multiple processes to function, so the kernel takes care of running the processes, starting and stopping them as requested, and handing out system resources.
* Linux software generally falls within any of these 3 categories
  * **Server Software**:  Softwares whose main purpose is to server other computers know as client
  * **Desktop Software**: Software which the end user can interract with directly.
  * **Tools**: A loose category of software that exists to make it easier to manage computer systems. Tools can help configure displays, provide a Linux shell that users type commands into, or even more sophisticated tools, called compilers, that convert source code to application programs that the computer can execute
### 3.2.2 - Server Applications
#### 3.2.2.1 - Web Server (Apache, NGINX) 
A web server hosts content for web pages, which are viewed by a web browser using the HyperText Transfer Protocol (HTTP) or its encrypted flavor, HTTPS. The web page itself can either be static or dynamic.

#### 3.2.2.2 Private Cloud Servers (ownCloud, Nextcloud)
#### 3.2.2.3 Database Servers
#### 3.2.2.4 Email Servers
* Mail Transfer Agent (MTA) - Sendmail and Postfix
* Mail Delivery Agent (MDA) AKA Local Delivery Agent.
* Post Office Protocol (POP) & Internet Message Access Protocol (IMAP)
#### 3.2.2.5 File Sharing 
* **Samba** : Samba allows a Linux machine to look and behave like a Windows machine so that it can share files and participate in a Windows domain.
* **Netatalk** : project lets a Linux machine perform as an Apple Macintosh file server. The native file sharing protocol for UNIX/Linux is called the Network File System (NFS). NFS is usually part of the kernel which means that a remote file system can be mounted (made accessible) just like a regular disk, making file access transparent to other applications.

### 3.3.1 Shells
The two main families are the Bourne shell and the C shell. The Bourne shell was named after its creator Stephen Bourne of Bell Labs. The C shell was so named because its syntax borrows heavily from the C language. As both these shells were invented in the 1970s, there are more modern versions, the Bourne Again Shell (Bash) and the tcsh (pronounced as tee-cee-shell). Bash is the default shell on most systems, though tcsh is also typically available.

Programmers have taken favorite features from Bash and tcsh and made other shells, such as the Korn shell (ksh) and the Z shell (zsh). 

### 3.5 Development Languages
A computer programmingg langage is just a tool that makes it easier to tell the computer what you want it to do. A library bundles common tasks into a distinct package that can be used by the developer examples includes ImageMagick, OpenSSL and the C Library.


## Chapter 4 - Open Source Softwares and Licensing
### 4.2 Open Source Licensing
there are 3 components to consider when buying a software
- **Ownership**: Who owns the intellectual property behind the sofware?
- **Money Transfer**: How does money change hands, if at all?
- **Licensing**: What do you get? What can you do with the software? 
Can you use it on only one computer? 
Can you give it to someone else?

the **End User License Agreement (EULA)**, is a custom legal document that you must click through, indicating your acceptance, in order to install the software.

the **GNU General Public License version 2 (GPLv2).** This license, among other things, says that the source code must be made available to anyone who asks and that anyone is allowed to make changes. One caveat to this is that if someone makes changes and distributes them, they must put the changes under the same license so that others can benefit.
GPLv2 also says that no one is allowed to charge for distributing the source code other than the actual costs of doing so (such as copying it to removable media).

**Free and Open Source Software (FOSS)** refers to software where this right has been given up; anyone is allowed to view the source code and redistribute it. Linus Torvalds has done that with Linux
* Free Software Foundations (FSF)
  * Copyleft
  * Tivoization
* Open Source Initiative (OSI)
  * Berkely Software Distribution (BSD)

## Chapter 5 - Command Line Skills
### 5.2 - Shell
The shell is the command line interpreter that translates commands entered by a user into actions to be performed by the operating system. If output is produced by the command, then text is displayed in the terminal. If problems with the command are encountered, an error message is displayed.

### Commands
* `type [command]`: shows the type of a command e.g `type cd` or `type -a echo `
* `;` use it to separate a succession of command to be run `ls; cd ..`
* `which [command]`: shows the location a command is installed/run from
* Variables [global or local] can only be called within double quotes e.g `echo "The path is $PATH" `
* `&&` acts a logical AND i.e the next command will be run only if the previous command was true. e.g 
  * `ls /etc/ppp && echo success` 
  * `ls /etc/junk && echo success`
* `||` acts as a logical OR which means the next command will be run depending on if the previous command was false (fails).
* Functions e.g 
```bash
function_name () {
  commands
}
```

### Labs
`whoami`: displays the user name of the current user
`uname` : displays information about the current system
`pwd` : diplays the parth of the current working directory
`history`: shows the history of commands you have entered so far. to run a command again use `!no` to excute the command e.g `!10` to excute the 10th command in the history
`alias` : display a list of user configured aliases for commands

## Chapter 6 - Getting Help
* Man Pages: are used to describe the features of commands.
  * `man [command]` e.g  `man ls`
  * `/` to search the man page. After entering the text to search for, hit `Enter` and use `n` and `Shift+N` to navigate.
  * use `q` to exit the man page.
  * By default, there are nine sections of man pages:
      1. General Commands
      2. System Calls
      3. Library Calls
      4. Special Files
      5. File Formats and Conventions
      6. Games
      7. Miscellaneous
      8. System Administration Commands
      9. Kernel Routines
  
  * `man -f command`: displays a list of manual entries for a command e.g `man -f write`
    * `man no command`: show the manual entry fo the no. provided. e.g:
      * `man 2 write` will list the write manual in the second page.
      * `whatis write` is same as `man -f write` on some linux distros

  * `man -k keyword` : is used to search for manual entry, when you don't know the exact name of the command. e.g :
    * `man -k copy` will show all the command that has copy in their summary/description.
    * `apropos copy` is the same as `man -k copy` 

  * `whereis command`: is used to search for the location and man page of a command.
  * `locate file/folder`: is used to search for the location of a file or directory. use `sudo updatedb`: to update the database of indexed files

* `info command`: similar to man but show a more detailed guide of a command e.g `info ls`
