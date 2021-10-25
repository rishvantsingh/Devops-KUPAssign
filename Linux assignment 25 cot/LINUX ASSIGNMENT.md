##                                  **LINUX ASSIGNMENT**  

### Question and Answers: 

#### \1. What is a GNU project?

Ans - Gnu project was bulit with an aim of creating a free operating system which can be free to run , use , update , change , copy   by anyone worldwide.

THe GNU project was comperised of many sub projects often reffered to as GNU packages.It is also referred to as GNU's not unix though it seemed to have the technical design of UNIX but unlike it is is a  free software. GNU Had a modular approach which led Linux kernel to be a part of it and together they deveoloped a free OS that is called as LINUX these days.

#### \2. What is the difference between Unix & Linux?

| UNIX                                                         | LINUX                                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| It is not an open source and can only be used by its copywriters with customised cost. | It is an open source OS which can be freely used by anyone . |
| Was developed manly for mainframes and servers.              | Linux can be used by anyone be it sudent , developer , home users , admixistrator etc. |
| It is CLI based                                              | It has both GUI and CLI.                                     |
| THe support of UNIX is there but not large as compared to linux because it comes under a proprietery. | LINUX has a large community support .                        |
| Few expamples of UNIX are OS X , Solaris                     | Examples are Ubuntu , Fedora , Red hat.                      |

#### \3. What do you mean by Integrity check of BIOS? Mention firmwares other than BIOS.

  It is done to check the bios has found the bootable resource or not.It checks various hardware bootable devices to check it.

It uses POST Power on self test. It checks whether the system is woking fine or not.If there is some error then it will give a beep.

There is  a firmware other than BIOS i.e UEFI.

#### \4. What is a UEFI?

UEFI stands for Unified Extensible Firmware Interface. It does the same job as a BIOS, but with one basic difference: it stores all data about initialization and startup in an .efi file, instead of storing it on the firmware.

This .efi file is stored on a special partition called EFI System Partition (ESP) on the hard disk. This ESP partition also contains the bootloader.

UEFI was designed to overcome many limitations of the old BIOS, including:



#### \5. What is the difference between BIOS & UEFI?

| BIOS                                                         | UEFI                                        |
| ------------------------------------------------------------ | ------------------------------------------- |
| BIOS only supports 2.2 terabytes.                            | UEFI supports drive sizes upto 9 zettabytes |
| Its not as fast as UEFI                                      | UEFI provides faster boot time.             |
| BIOS has drive support stored in its ROM, so updating BIOS firmware is a bit difficult. | UEFI has discrete driver support            |
|                                                              | UEFI provides faster speed and stability    |

#### \6. When should you go for Ubuntu & when for other systems?

UBUNTU is a linux based os so if someone is planning for a heavily secured and fast os then he / she should go for Ubunut. It has an elegant GUI thus good for transitioning from windows aor mac.

#### \7. List various linux distributions

Various lINUX distributions are 

& their use cases.

1. Ubuntu: It is based on Debian. It has an elegant GUI and thus designed to help people who transitioned from windows or mac to Linux.
2. Debian: Debain is the mother of distros. Ubuntu, Linux Mint are based on Debian. It has high stability and thus can be used in production servers.
3. RHEL: Red Hat Enterprise Linux. It is designed for commercial and enterprise purposes. It has a paid support contract.
4. Centos: It is based on Red Hat distro. Except it is free and does not provide the paid support contract.
5. Fedora: Based on Red Hat distro. Has all the new features and updates and hence less stable.
6. Kali Linux: Developed for pentration testing.

#### \8. What does a systemd.unit(5) means?

It represents the section of a particular man page. That means it is the 5th sec of the page.

Man Pages are divided into 8 sections.

- User Commands : Commands that can be run from the shell by a normal user 
- System Calls: Programming functions used to make calls to the Linux kernel 
- C Library Functions: Programming functions that provide interfaces to specific programming libraries. 
- Devices and Special Files: File system nodes that represent hardware devices or software devices. 
- File Formats and Conventions: The structure and format of file types or specific configuration files. *
- File Formats and Conventions: The structure and format of file types or specific configuration files. 
- Games: Games available on the system 
- Miscellaneous: Overviews of miscellaneous topics such as protocols, filesystems and so on. 
- System administration tools and Daemons:Commands that require root or other administrative privileges to use.



#### \9. What are getty commands and uname command?

The **uname command** is used to display information about the system. To know the operating system release , the version , etc we use the uname command.

THe getty command is run by the init command and is used to set and manage the terminal lines and port.Whenever it detects a virtual connection it runs the login command and authenticates the user.



#### \10. What is squashfs file system?

When working with small embedded type linux system each nd every granule of the storage device is necessary so compression is used everywhere possible and also the archieve of the compressed file is stored.So squashfs brings this thimg to another level.

It is a read only file system that lets us compress the whole file and directories and lets us write it in the other partitions and directly mount it.

#### \11. What are /dev/loop and /dev/tty ?

dev/tty is a special file, representing the terminal for the current process.

dev/tty is a loop device file which is used to mount snaps and images.

#### \12. What are Linux Signals?

A signal is sent when some unusual even occurs in the normal wokring .

Now in linux there are several signals that have their own meaning.

For example: -

SIGNIT - 1 - it is sent whe ctrl+c is pressed i.e an interrupt signal

SIGQUIT - 3- It is sent when ctrl +d is pressed i.e a quit signal is pressed.

To see all the signals we can use kill -l

#### \13. What is the purpose of creating and using hidden files.

 He hidden files play a very vital role in systems.

- They are hidden so they cannot be accidently deleted.
- They provide a safe access of data that is we can prevent data from unauthenticated soure.
- It helps in preservation of utilities like the secured data.

#### 

#### \14. How ext4fs is faster/better?

Ext4 has a large filesystem support , improved resistance to fragmentation, higher performance, and improved timestamps.

Ext4 uses 48-bit internal addressing, making it theoretically possible to allocate files up to 16 TiB on filesystems up to 1,000,000 TiB (1 EiB).

In ext4 the storage blocks are allocated before writing them on the disk. So reading and writing becomes easier.

#### \15. What is swap & swap memory?

swap - Swap is a space on a disk that is used when the amount of physical RAM memory is full. When a Linux system runs out of RAM, inactive pages are moved from the RAM to the swap space.

swap memory - The space occupied by these inactive files is called swap memory.

\16. How to mount a file system?

To mount a particular file system for example

```
mount [OPTION...] DEVICE_NAME DIRECTORY
```

#### \17. Mention a ZFS use case.

ZFS  is better at protecting and securing our data and can protect our data against corruption. It can manage data better than ext4. SO it is used in enterprises and large data working backgrounds;

#### \18. How to check the port number of a process?

- netstat -lntp

#### \19. What is unix time sharing (UTS)?

It is a namespace which allows a same system to appear to processes with different hostname and different domain.

#### \20. What are control groups?

Cgroups allows processes to be organized into hierarchial order where then usage can be limited and monitored.It is used in resurce management.

It is a Linux kernel feature that limits, accounts for, and isolates the resource usage (CPU, memory, disk I/O, network, and so on) of a collection of processes.

#### \21. What is the difference between sbin & usr/sbin?

Sbin contains the binaries of commands which require root priviledges. The /sbin directory under root directory is available for all the users and are used when a system is booted and the usr partition is not mounted.

#### \22. Examples of awk, grep and sed

awk - WIth awk we can

- Define variables.

- Use string and arithmetic operators.

  fOr example

awk - $ awk '{print "Welcome to knoldus"}' - It prints the statement.

**grep** - It is used to search for a string in a particular file or stream.

for exmple - grep option pattern filename

grep -i "a" a.txt

**sed**- sed is a stream editor .It can do lot of funtions such as replacing , finding , insertion , deletion , replacement.

example - sed 's/string/stringtobereplaced/g' filename

#### 

#### \23. How many tables are there in iptables?

There are total of five tables in iptable. They are:

**1- Filter Table** - It is the default table of iptable.If you don't specify your table then then this table is made.

It has three chains.

Input chain - It basically defines the incoming to firewall for packages that come locally to the server.

Output chain -It defines outgoing the firewall for packages that leave the local server.

forward chain -This is for package routed through local server.

**2- Mangle table** - It is used for specialised packet alteration.

Mangle table has the following built-in chains.

- PREROUTING chain - This means that the packets are altered before routing.That is when the packet comes the destination ip can be changed before sending and helps to transform the ip to something local system ip.
- OUTPUT chain -It defines outgoing the firewall for packages that leave the local server.
- FORWARD chain - This is for package routed through local server.
- INPUT chain - It basically defines the incoming to firewall for packages that come locally to the server.
- POSTROUTING chain - This Alters packets after routing. i.e Packet translation happens when the packets are leaving the system. This helps to translate the source ip address of the packets to something that might match the routing on the desintation server.

**3- Raw table** - It is used only for configuring packets so that they are exempt from connection tracking.

 Raw table has the following built-in chains.

- PREROUTING chain
- OUTPUT chain

**4-NAT table** - It is used for networking address translation. For example port forwarding.

**5- Security table** - This table is used for Mandatory Access Control (MAC) networking rules, such as those enabled by the **SECMARK** and **CONNSECMARK** targets.

#### 

#### \24. What is prot, opt, in, out, source & destination?

***Target:-*** This defines what action needs to be done on the packet (ACCEPT,DROP,etc..)'

**opt**:- Special options for that specific rule.

**in**`: Name of input interface via which the packet is received

**out`**: Name of output interface via which the packet will be send

***prot:-*** This defines the protocol (TCP,IP) of the packet.

***source:-*** This tells the source address of the packet.

***destination:-*** This defines the destination address of the packet.

#### \25. Why rules are added to the top?

Rules are added to top becuase whenever the packets are passed from the first rule it does not check the bottom rules.

#### \26. What type of rules we can add to the iptables?

Accept - It lets the incoming packets from the source

-Reject - It lets the other end know what port is unreachable.

-Drop- It is used for connections to hosts we don’t want people to see.

#### \27. Can we block a website by its domain name only?

Yes we can block by command .

#### \28. How can we persist rules in iptables?

1. Add rules to the iptables according to your requirment.

2. Verify that all the rules are present using the command “**iptables -L**“.

3. Save the iptables.

   ```
   # service iptables save
   ```

   4-Restart the service.

   ```
   # service iptables restart
   ```

   1. Making service permanently **ON** using chkconfig.

   ```
   # chkconfig iptables on
   ```

#### \29. How can we save rules in iptables?

This we can do by using persistent package

```
sudo /etc/init.d/iptables-persistent save 
sudo /etc/init.d/iptables-persistent reload
```

#### 

#### \30. What is the difference between ufw & iptables.

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| ufw                                                          | iptables                                                     |
| UFW is a simplified firewall mechanism that is implemented on top of iptables. | Iptables is a kernel level ip filtering mechanism. It does allow you to make routing decisions and so on on IP packets. |
| UFW is not as flexible but is easier to configure for common scenarios. | To use IPtables you need to understand TCP/IP connections, more complicated protocols |
|                                                              |                                                              |

#### \31. What are public & private keys?

| public keys                                                  | private keys                                                 |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| A [public key] is that is copied to the SSH server(s). Anyone with a copy of the public key can encrypt data which can then only be read by the person who holds the corresponding private key. | A [private key is that remains (only) with the user. The possession of this key is proof of the user's identity. Only a user in possession of a private key that corresponds to the public key at the server will be able to authenticate successfully. |

#### \32. How does ssh work?

SSH works by making the use of client server model.It helps in securing the making the connection encrypted and allows to authenticate two remote system.

It woks by public key authention. When a client autheticates to a remote server a public key is generated and it is stored in rsa form from which while connecting it

#### \33. What is the difference between HTTP & HTTPS.

| HTTP                                                         | HTTPS                                                        |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| The HTTP protocol stands for Hypertext Transfer Protocol,    | HTTPS stands for Hypertext Transfer Protocol Secure.         |
| The HTTP protocol is not secure protocol as it does not contain SSL (Secure Sockets Layer), which means that the data can be stolen when the data is transmitted from the client to the server.\ port number 80, | the HTTPS protocol contains the SSL certificate that converts the data into an encrypted form, so no data can be stolen in this case as outsiders do not understand the encrypted text. port number 443 |

#### 

#### \34. What is SSL?

SSL stands for Secure Sockets Layer and, is used for keeping an internet connection secure and safeguarding any sensitive data that is being sent between two systems

#### \35. What is the difference between apt update & apt upgrade.

| apt update                                                   | apt upgrade                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| apt update is used to download package information from all configured sources. | apt upgrade is the command used to download and apply any available updates to your packages in a safe manner by not removing packages that are previously installed in a given Linux system |

#### \36. What do repositories contain in a Linux system?

THe repositores contain all the source codes of the version file and also contains the configuration files.

#### \37. What are the package managers used in Linux?

THe package managers used in Linux are 

- apt 
- dpkg
- snap

#### \38. What does the number represent after the file permissions?

It represents the number of files.

\39. What is the difference between apt and apt-get?

| apt                                                          | apt-get                                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| apt is a subset of apt-get and apt-cache commands providing necessary commands for package management | `apt-get` may be considered as lower-level and "back-end", and support other APT-based tools. |

#### \40. How can I give access to someone to my AWS instance?

We can achieve this by adding the public key of the user to the aws instance authorized_key.

#### \41. What are daemon applications?

These are the applicaions that run in backgorund .All daemons have their name end with d .

#### \42. What does a ".d" represent after a filename?

"d" stands for directory and such a directory is a collection of configuration files which are often fragments that are included in the main configuration file. The point is to compartmentalize configuration concerns to increase maintainability.

#### \43. What happens when a pem file gets deleted?

We cannot the acces the aws instance if the pem is deleted.

#### \44. What information is stored in the /etc/host file?

The host file stores the hostname and ip address.This file is an ASCII text file. It contains **IP addresses separated by a space and then a domain name**. Each address gets its own line.

#### \45. What is SCP & what does this command do?

The SCP command or **secure copy allows secure transferring of files in between the local host and the remote host** or between two remote hosts.

command: - scp -i pem_file file_name ubuntu@ip destiantion

#### \46. How port forwarding works?

**Port forwarding** is a technique that is used to allow external devices access to computers services on private networks. Local port forwarding is the most common type of port forwarding. It is used to let a user connect from the local computer to another server, i.e. forward data securely from another client application running on the same computer as a [Secure Shell](https://en.wikipedia.org/wiki/Secure_Shell) (SSH) client

#### \47. How can we connect without IP to AWS instance?

We set `Host` , `User`, `IdentityFile` and `Hostname` in the `.ssh/config` file. The syntax is

```
Host myserver
HostName 18.118.157.232
User ubuntu
IdentityFile ~/Downloads/demo-pair.pem
```

#### \48. What is an ssh agent?

SSH agent basically holds the priavte keys which is used for authentication publically. If the priavte key is encrypted then it helps to authenticate automatically.We just need to put the passphrase only once.THe ssh agent caches the key for us.

#### \49. Create a unit file for any application.

I have created and uploaded in the same repo.

#### \50. What is RHEL?

RHel stands for Red Hat ENterprise Linux is a linux based operaing system.It is a commercially available linux os manily designed for businesses who need more functionality and high security while working at it.

RHEL provides a better and faster approach.



