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