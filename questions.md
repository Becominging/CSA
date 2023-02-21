# 一些问题



\1) Why should we consider AWS? How would you convince a customer to start using AWS?
Primary advantage is going to be cost savings. As a customer support engineer your job role involves talking to current customers, prospective customers to help them determine if they really have to move to AWS from their current infrastructure that can be either onsite (or) in another hosting platform. In addition to providing convincing answer in terms of cost savings it would be better if you give them real simple explanation of flexibility, elastic capacity planning that offers option of pay as you use infrastructure, easy to manage AWS console etc
\2) What is your current job profile?How would you add value to customer?
Though AWS is looking to hire fresh talent for cloud support engineer openings, if you have some work experience in infrastructure side of business say system administrator, network administrator, database administrator, firewall administrator, security administrator, storage administrator etc you are still a candidate to be considered for interview.
All they are looking for is infrastructure knowledge in overall, little knowledge about different tech stack , how they inter-operate, what will it be like once the infrastructure is in web rather than physical data center.
If you don’t have experience with AWS don’t worry. Try to leverage the ways and means you did adopt to solve customer support calls both internal and external to let them know how you can bring value to the table.
Have some overview on how different components of infrastructure interact.
AWS wants to know your pro-active measure towards customer relationship. Say, if you are going to discuss a project or an issue with customer , it would be better if you have some preparatory work that comes handy rather than being reactive. Value addition comes in terms of recommending the best solution , utilization of services in AWS that will help them make decision easy and fast
\3) Do you know networking?
Make sure you can be from many different backgrounds say from development, infrastructure, QA, customer support , network administration, system administration, firewall administration, system administration etc. You should know networking. Cloud is network based and to fix the application issues escalated, networking knowledge is very important
\4) What networking commands do you make use of on daily basis to fix issues?
When we work with servers be it physical or virtual first command that comes handy to locate the request response path taken would be traceroute. In windows systems equivalent command is tracert
There are some more important interesting commands – ping, ipconfig, ifconfig that talks about network communication, network address, interface configuration etc
DNS commands – nslookup, Lookup of /etc/resolv.conf file in Linux systems to get details on DNS
\5) What is the advantage of using TCP protocol?
TCP is used to exchange data reliably . IT used mechanisms of sequence and acknowledgment, error detection, error recovery. This comes with advantage of reliable application but comes with cost of hit in transmission time
\6) What is UDP?
User datagram protocol called UDP is a connection less protocol that can be used for fast efficient applications that need less time compared to TCP
\7) Do you know how an internet works in your environment?
This can be your home or office. Learn more on modem and its utilization in connection establishment
\8) What is a process? How do you manage processes in Linux:-
In Linux/Unix based OS process is started or created when a command is issued. In simple terms while a program is running in an OS an instance of the program is created. This is the process. To manage the processes in Linux process management commands come handy
ps – this is the commonly used process management command to start with. ps command provides details on currently running active processes
top – This command provides details on all running processes. ps command lists active processes whereas top lists all the processes (i.e) activity of processor in real-time. This includes details on processor and memory being used
kill – To kill a process using the process id kill command is used. ps command provides details on process id. To kill a process issue
kill pid
killall proc – This command is same as kill command. To kill all the processes by name proc we can use this
\9) Give details on foreground and background jobs command in Linux:-
fg – this command brings most recent job to foreground. Typing the command fg will resume most recently suspended job
fg n – This command brings job n to the foreground. If a job is recently back grounded by typing fg 1 this can be brought foreground
bg – This command is used to resume a suspended program without bringing it to foreground. This command also provides details on list of stopped jobs as well as current background jobs
\10) How to get details on current date and time in Linux?
Make use of the command date that shows details on current date and time. To get current month’s calendar use cal command
uptime – shows current uptime
\11) What is difference between command df and du?
In linux both df and du are space related commands showing system space information
df – this command provides details on disk usage
du – To get details on directory space usage use this command
free – this command shows details on memory and swap usage
\12) What are the different commands and options to compress files in Linux?
Lets start with creating a tar and name it test.tar containing the needed files
tar cf test.tar files
Once the tar is available, uploaded on AWS there is a need to untar the files. Use the command as follows:
tar xf file.tar
We can create a tar with gzip compression that will minimize the size of files to be transferred and creates test.tar.gz at the end
tar czf test.tar.gz files
To extract the gzipped tar compressed files use the command:
tar xzf test.tar.gz
Bzip2 compression can be used to create a tar as follows
tar cjf test.tar.bz2
To extract bzip2 compressed files use
tar xjf test.tar.bz2
To simply make use of gzip compression use
gzip testfile – This creates testfile.gz
To decompress testfile.gz use gzip -d testfile.gz
\13) Give examples on some common networking commands you have made use of?
Note that AWS stack is primarily dependent on linux and over the cloud architecture makes it heavily network dependent. As a result AWS interview could be related to networking irrespective of your system admin, database admin, bigdata admin background. Learn these simple networking commands:
When a system is unreachable first step is to ping the host and make sure it is up and running
ping host – This pings the host and output results
Domain related commands as AWS has become preferred hosting for major itnernet based companies, SaaS firms
To get DNS information of the domain use – dig domain
To get whois information on domain use – whois domain
Host reverse lookup – dig -x host
Download file – wget file
To continue stopped download – wget -c file

\14) What is your understanding of SSH?
SSH the secure shell is widely used for safe communication. This is a cryptographic network protocol used for operating network services securely over an unsecured network. Some of the commonly used ssh commands include
To connect to a host as a specified user using ssh use this command:
ssh username@hostname
To connect to a host on a specified port make use of this command
ssh -p portnumber username@hostname
To enable a keyed or passwordless login into specified host using ssh use
ssh-copy-id username@hostname
\15) How do you perform search in Linux environment?
Searching and pattern matching are some common functions that typically happens in Linux environment. Here are the Linux commands:
grep – Grep command is the first and foremost when it comes to searching for files with pattern. Here is the usage:
grep pattern_match test_file – This will search for pattern_match in test_file
Search for pattern in directory that has set of files using recursive option as follows – grep -r pattern dir – Searches for pattern in directory recursively
Pattern can be searched in concatenation with another command (i.e) output of a command can be used as input for pattern search and match – first command| grep pattern
To find all instances of a file use locate command – locate file
\16) Give details on some user related commands in Linux:-
Here are some user related Linux commands:
w – displays details on who is online
whoami – to know whom you are logged in as
finger user – displays information about the user
\17) How to get details on kernel information in Linux?
uname -a command provides details on kernel information
\18) How to get CPU and memory info in Linux machine?
Issue the following commands:
cat /proc/cpuinfo for cpu information
cat /proc/meminfo for memory information
\19) What are the file system hierarchy related commands in linux?
File system hierarchy starting with raw disks, the way disks are formatted into files, files are grouped together as directory all are important for cracking AWS interview. Here are some file system hierarchy related commands that come handy
touch filename – creates a file with name filename. This command can also be used to update a file
ls- lists the directories
ls -al – All files including hidden files are listed with proper formatting
cd dir – change to specified directory
cd – Changes to home directory
pwd – called present working directory that shows details on current directory
Make a new directory using mkdir command as follows – mkdir directory_name
Remove file using rm command – rm file – removes file
To delete directory use -r option – rm -r directory_name
Remove a file forcefully using -f option – rm -f filename
To force remove directory use – rm -rd directory_name
Copy the contents from one file to another – copy file1 file2
Copy the contents across directory use – cp -r dir1 new_dir – If new directory does not exist create this first before issuing copy command
Move or rename a file using mv command – mv file1 new_File
If new_Dir is a file that already exists new_File will be directory into which file1 will be moved into
more filename – output the contents of the file
head file – output the first 10 lines of the file
tail file – output the last 10 lines of the file
tail -f filename – output the contents of the file as it grows, to start with display last 10 lines
Create symbolic link to a file using ln command – ln -s file link – called soft link
\20) What command is used for displaying manual of a command?
Make use of the command man command_name
\21) Give details on app related commands in linux:-
which app – shows details on which app will be run by default
whereis app – shows possible locations of application
\22) What are the default port numbers of http and https?
Questions on http and https port number is first step in launching webapp while customer reports an issue
Default port number of http is 80 (or) 8080
Default port number of https is 443
\23) What is use of load balancer?
Load balancer is used to increase the capacity and reliability of applications. What capacity means is number of users connecting to applications. Load balancer distributes the traffic network and application traffic across many different servers increasing application capacity
\24) What is sysprep tool?
System preparation tool comes as free tool with windows that can be accessed from %systemroot%\system32\sysprep folder. IT is used to duplicate, test and deliver new installation of windows based on established installation
\25) User is not able to RDP into server. What could be the reason?
Probable reason is that user is not part of remote desktop users local group of the terminal servers
\26) How would you approach a customer issue?
Most work of AWS support engineer involves dealing with customer issue.As with any other support engineer AWS engineer should follow approach of question customer, listen to them, confirm what you have collected. This is called QLC approach much needed step to cover details on issue description and confirm it
\27) What types of questions can you ask customer?
A support engineer can ask two types of questions
\1) Open ended questions – In this case your question will be single statement, answer you expect from customer is detailed
\2) Closed questions – In this case your question will have answers yea (or) No, true (or) false type answers, single word answer in some cases
\28) How do you consider customer from AWS technology perspective?
Even though the customer can be long standing customer of AWS, always think of customer as common man with no knowledge of AWS to talk more to them, explain more details to them to get correct issue description statement
\29) Give details on operators in linux?
\> – greater than symbol is input re-direction operator used to write content as input into file. Typically this is used to redirect the output of command into logfile. IF file already exists the contents are overwritten and only last recent content is retained
\>> – this is same as input redirection except that this is appending content of a file if the file already exists
\30) Explain difference between hardlink and softlink in simple terms?
Hardlink is link to inode that talks about file contents, softlink is link to filename. If filename changes the changes are not reflected. For both hard and soft link ln command is used. In case of hardlink it will be simply ln, for soft link ln -s option is used
\31) What are some common linux commands AWS engineer should be aware of?
\1) cat – This is plain simple command to access a file in UNIX
\2) ls – Provides details on list of files and directories
\3) ps – The process command provides details on list of processes in the system
\4) vmstat – Virtual memory statistics comes handy during performance tuning
\5) iostat – Command to determine I/O issues
\6) top – This command provides details on top resource consuming processes
\7) sar – This is a UNIX utility mainly used for tuning purpose
\8) rm – This command is used to remove files
\9) mv – moving the files and directories
cd – Enables us to change directories
date – gives us the time and date
echo – we can display text on our screen
grep – It is a pattern recognition command.It enables us to see if a certain word or set of words occur in a file or the output of any other command.
history – gives us the commands entered previously by us or by other users
passwd – this command enables us to change our password
pwd – to find out our present working directory or to simply confirm our current location in the file system
uname – gives all details of the system when used with options. We get details including systemname,kernel version etc.
whereis – gives us exact location of the executable file for the utility in the question
which – the command enables us to find out which version(of possibly multiple versions)of the command the shell is using
who – this command provides us with a list of all the users currently logged into the system
whoami – this command indicates who you are logged in as. If user logs in as a userA and does a su to userB,whoami displays userA as the output.
man – this command will display a great detail of information about the command in the question
find – this command gives us the location of the file in a given path
more – this command shows the contents of a file,one screen at a time
ps – this command gives the list of all processes currently running on our system
cat – this command lets us to read a file
vi – this is referred to as text editor that enables us to read a file and write to it
emacs- this is a text editor that enables us to read a file and write to it
gedit – this editor enables us to read a file and write to it
diff – this command compares the two files, returns the lines that are different,and tells us how to make the files the same
export – we can make the variable value available to the child process by exporting the variable.This command is valid in bash,ksh.
setenv – this is same as export command and used in csh,tcsh
env – to display the set of environment variables at the prompt
echo <$variablsname> – displays the current value of the variable
source – whenever an environment variable is changed, we need to export the changes.source command is used to put the environment variable changes into immediate effect.It is used in csh,tcsh
.profile – in ksh,bash use . .profile command to get same result as using source command
set noclobber – to avoid accidental overwriting of an existing file when we redirect output to a file.It is a good idea to include this command in a shell-startup file such as .cshrc
\32) What are the considerations while creating username/user logins for Security Administration purpose?
It is a good practice to follow certain rules while creating usernames/user logins
\1) User name/user login must be unique
\2) User name/user login must contain a combination of 2 to 32 letters, numerals, underscores(_),hyphens(-), periods(.)
\3) There should not be any spaces/tab spaces while creating user name/usr logins
\4) User name must begin with a letter and must have atleast one lowercase letter
\5) Username must be between three to eight characters long
\6) It is a best practice to have alphanumeric user names/user logins. It can be a combination of lower case letters, upper case letters, numerals, punctuation
\33) Give details on /etc/profile the system profile file and its usage in linux environment:-
.This is another important UNIX system administration file. This file has much to do with user administration. This file is run when we first log into the system.This is system profile file. After this user profile file is run. User profile is the file wherein we define the users environment details.Following are teh different forms of user profile files :
.profile
.bash_profile
.login
.cshrc
/home/username is the default home directory.User’s profile file resides in the user’s home directory.
\34) How to perform core file configuration in Linux environment?
Lets consider a linux flavor say solaris. Core File Configuration involves the following steps. We need to follow the steps given below to configure the core file.
\1) As a root user, use the coreadm command to display the current coreadm configuration :
\# coreadm
\2) As a root user, issue the following command to change the core file setup :
\# coreadm -i /cores/core_new.%n.%f
\3) Run the coreadm command afain to verify that the changes has been made permanent
\# coreadm
The O/P line “init core file pattern : ” will reflect the new changes made to the corefile configuration.
From solaris 10 onwards, coreadm process is configured by the Service Management Facility (SMF) at system boot time.We can use svcs command to check the status .The service name for coreadm process is :
svc:/system/coreadm:default
\35) How do you configure or help with customer printer configuration?
Administering Printers details the steps needed to administer a printer.
Once the printer server and printer client is set up, we may need to perform the following administrative tasks frequently :
\1) Check the status of printers
\2) Restart the print scheduler
\3) Delete remote printer access
\4) Delete a printer
\36) How is zombie process recognized in linux and its flavors? How do you handle zombie process in linux environment?
Zombie Process in UNIX/LINUX/Sun Solaris/IBM AIX is recognized by the state Z.It doesn’t use CPU resources.It still uses space in the process table.
It is a dead process whose parent did not clean up after it and it is still occupying space in the process table.
They are defunct processes that are automatically removed when a system reboots.
Keeping OS and applications up to date and with latest patches prevents zombie processes.
By properly using wait() call in parent process will prevent zombie processes.
SIGCHLD is teh signal sent by child to parent upon task completion and parent kills child(proper termination).
kill -18 PID – Kills childs process
\37) What is the use of /etc/ftpd/ftpusers in Linux?
/etc/ftpd/ftpusers is used to restrict users who can use FTP(File Transfer Protocol).Ftp is a security threat as passwor is not encrypted while using ftp. ftp must not be used by sensitive user accounts such as root,snmp,uucp,bin,admin(default system user accounts).
As a security measure we have a file called /etc/ftpd/ftpusers created by default. The users listed in this file are not allowed to do ftp.The ftp server in.ftpd reads this file before allowing users to perform ftp. If we want to restrict a user from doing ftp we may have to include their name in this file.
\38) Have you ever helped a customer restore a root file system in their environment?
Restoring root file system (/)  provides steps we need to follow to restore the root file system (/ system) in SPARC and x86 (intel) machines.
\1) Log in as root user. It is a security practice to login as normal user and perform an su to take root user (super user) role.
\2) Appearance of # prompt is an indication that the user is root
\3) Use who -a command to get information about current user
\4) When / (root filesystem) is lost because of disk failure. In this case we boot from CD or from the network.
\5) Add a new system disk to the system on which we want to restore the root (/) file system
\6) Create a file system using the command :
newfs /dev/rdsk/partitionname
\7) Check the new file system with the fsck command :
fsck /dev/rdsk/partitionname
\8) Mount the filesystem on a temporary mount point :
mount /dev/dsk/devicename /mnt
\9) Change to the mount directory :
cd /mnt
\10) Write protect the tape so that we can’t accidentally overwrite it. This is an optional but important step
\11) Restore the root file system (/) by loading the first volume of the appropriate dump level tape into the tape drive. The appropriate dump level is the lowest dump level of all the tapes that need to be restored. Use the following command :
ufsrestore -rf /dev/rmt/n
\12) Remove the tape and repeat the step 11 if there is more than one tape for the same level
\13) Repeat teh step 11 and 12 with next ddump levels. Always begin with the lowest dump level and use highest ump level tape
\14) Verify that file system has been restored :
la
\15) Delete the restoresymtable file which is created and used by the ufsrestore utility :
rm restoresymtable
\16) Change to the root directory (/) and unmount the newly restored file system
cd /
umount /mnt
\17) Check the newly restored file system for consistency :
fsck /dev/rdsk/devicename
\18) Create the boot blocks to restore the root file system :
installboot /usr/platform/sun4u/lib/fs/ufs/bootblk /dev/rdsk/devicename — SPARC system
installboot /usr/platform/`uname -i`/lib/fs/ufs/pboot /usr/platform/`uname -i`/lib/fs/ufs/bootblk /dev/rdsk/devicename — x86 system
\19) Remove the last backup tape, and insert a new tape onto which we can write. Make a dump level 0 backup of the newly restored system by issuing the following command :
ufsdump 0ucf /dev/rmt/n /dev/rdsk/deviceName
This step is needed because ufsrestore repositions the files and changes the inode allocations – the old backup will not truly represent the newly restored file system
\20) Reboot the system :
\#reboot (or)
\# init 6
System gets rebooted and newly restored file systems are ready to be used.
\21) What is the monitoring and reporting tool that comes as part of AWS console?
Cloudwatch the tool listed under management section of AWS console helps with monitoring and reporting emtrics in AWS environment. Following metrics can be monitored as part of cloudwatch including
\1) CPU
\2) Disk utilization
\3) Network
\4) Status Check
In addition to the above mentioned metrics RAM the custom metric can be monitored using cloudwatch
\22) Give details on status check in cloudwatch?
In an AWS environment status of both instance and system needs to be monitored. As such there are system status check as well as instance status check sections associated with each and every EC2 instance. As the name implies system status check makes sure that physical machines on which the instances have been hosted is in good shape. Instance status check is at the EC2 instance which literally translates to virtual machine in AWS environment
\23) What happens if a failure is reported in status check section of AWS?
Depending on what type of failure has been reported following actions can be taken:
In case of system failure – Restart the virtual machine. In AWS terms, restart the EC2 instance. This will automatically bring up the virtual machine in a physical hardware that is issue free
Instance Failure – Depending on the type of failure reported in EC2 instance this can be stopping and starting of virtual machine to ix the issue. In case of disk failure appropriate action can be taken at operating system level to fix the issues
\24) What is an EC2 instance in AWS?
This is the basic component of AWS infrastructure. EC2 translates to Elastic compute cloud. In real-time this is a pre-built virtual machine template hosted in AWS that can be chosen, customized to fit the application needs
This is the prime AWS service that eliminates a business necessity to own a data center to maintain their servers, hosts etc
\25) What is an ephemeral storage?
An ephemeral storage is a storage that is temporary (or) non-persistent
\26) What is the difference between instance and system status check in cloudwatch?
An instance status check checks the EC2 instance in an AWS environment whereas system status check checks the host
\27) What is the meaning of EBS volume status check warning?
An EBS volume is degraded or severly degraded. Hence, a warning in an EBS environment is something that can’t be ignored as with other systems
\28) What is the use of replicalag metric in AWS?
Replicalag is a metric used to monitor the lag between primary RDS the relational database service a database equivalent in AWS environment and the read replica the secondary database system that is in read only mode
\29) What is the minimum granularity level that a cloudwatch can monitor?
Minimum granularity that cloudwatch can monitor is 1 minute. In most real-time cases 5 minute metric monitoring is configured
\30) What is the meaning of ebs volume impaired ?
EBS volume impaired means that the volume is stalled or not available
\31) Where is ELB latency reported?
In cloudwatch the latency reported by elastic load balancer ELB is available
\32) What is included in EC2 instance launch log?
Once the EC2 instance is created, configured and launched following details are recorded in instance launch log:
Creating security groups – The result needs to be Successful. In case of issues the status will be different
Authorizing inbound rules – For proper authorization this should show Successful
Initiating launches – Again this has to be Successful
At the end we see a message that says Launch initiation complete
\33) What will happen once an EC2 instance is launched?
After the EC2 instance has been launched it will be in running state. Once an instance is in running state it is ready for use. At this point usage hours which is typically billable resource usage starts. This keeps accruing until we stop or terminate our instance. NExt immediate step is to view instance
\34) What is maximum segment size (mss)? How is this relevant to AWS?
The maximum segment size is the important factor that determines the size of an un fragmented data segment. AWS is cloud based and the products hosted are accessed via internet connection. For data segments to successfully pass through all the router during transit their size should be acceptable across routers. If they grow big the data segments get fragmented. This eventually leads to network slowness
\35) How does a load balancer check the EC2 instance availability in an AWS environment?
Periodically load balancer sends pings, attempts connections, send requests to EC2 instances to cehck their availability. Often these tests are referred as health checks in an AWS environment
\36) Give details on health check and status of instances in an AWS environment :-
In an AWS environment to check the status of EC2 instances the load balancer periodically sends pings, attempts connection, sends requests to EC2 instances. This process is referred to as health check in an AWS environment
If an EC2 instance is healthy and functioning normal at the time of health check the status will be InService
If an instance does not respond back this is unhealthy and its status will be OutOfService
\37) What are the instances that are candidates to be part of health check?
If an instance is registered with a load balancer this is a candidate under health check process in AWS. This covers instances that are in both healthy and unhealthy statuses which are typically InService and OutOfService respectively
\38) What happens when an instance in an AWS environment has been found to be in an unhealthy state?
The requests will not be routed to unhealthy instances by load balancer. Once the instance health is restored back to healthy status requests are routed here
\39) What is IPSec?
IPSec refers to the internet protocol security that is used to securely exchange data over public network that no-one can view and read except the intended parties. IPSec makes use of two mechanisms that work together to exchange data in a secure manner over the public networks. Though both of these mechanisms are not mandate we can use just one or both togetehr. The two mechanisms of IPSec are
Authentication header – Used to digitally sign the entire contents of each packet that protects against tampering, spoofing, replay attacks. The major disadvantage of authentication header is that though this protects data packets against tampering the data is still visible to hackers. To overcome this ESP can be used
Encapsulating Security Payload – ESP provides authentication, replay-proofing and integrity checking by making use of 3 components namely ESP header, ESP trailer, ESP authentication block
\40) What are the many different types of IPSec modes?
Tunnel more, transport mode are the two modes that we can configure IPSEc to operate in.Tunnel mode is the default mode and used for and used for communication between gateways like routers, ASA firewalls (or) at an end-station to a gateway. Transport mode is used for end-to-end communication between a client and a server, between a workstation and a gateway like telnet connection, remote desktop connection between a workstation and server over VPN etc
\41) In a class B network give relationship between network /count and number of hosts possible :-
network
/count No of hosts possible
16 65536
17 32768
18 16384
19 8192
20 4096
21 2048
22 1024
23 512
24 256
25 128
26 64
27 32
28 16
29 8
30 4
\42) In a class C network give relationship between network /count and number of hosts possible :-
network
/count No of hosts possible
24 256
25 128
26 64
27 32
28 16
29 8
30 4
\43) You are a DBA and have been assigned task of migrating oracle database to AWS with minimal to no impact to source database. How will you achieve this?
Make use of Database Migration Service. This will help you migrate databases securely and easily. This tool enables live migration of data making sure source database is up and running during migration
\44) Which AWS service will you make use of to monitor CPU utilization of an EC2 resource in AWS environment?
AWS Cloudwatch is a monitoring service that can be used for management as well in an AWS environment. We can get data insights to monitor system performance and optimize resource utilization in an AWS environment
\44) Give details on some AWS terminologies you need to be aware of as support engineer :-
Here are some common terminologies that you will come across in your daily job
EC2 instance – This is how the virtual machine is referred to in an AWS environment
Region – The physical geographical locations that host AWS datacenters is referred to as region. This keeps expanding with growth of AWS
RDS – The database related service commonly called as relational database services
S3- The storage service from AWS
EBS – The elastic block storage, another storage option from AWS
Availability zone – Commonly referred to as AZ
Virtual private cloud – Commonly called as VPC is datacenter in virtual format in AWS
\45) What is use of wireshark?
This is a open-source packet analyzer tool commonly used to monitor network traffic coming in and out of the servers hosting applications. At times is is used to monitor and make sure there are no security threats in this system
AWS support engineer interview for database administrators:
———————————————————–
Being an Oracle DBA, with current job market condition I’ve always been in search of perfect technology that will help us sustain in this tough job market with lots of lay-offs. Based on changing demography of IT infrastructure, I thought all the infrastructure professionals including system administrators both linux, unix, aix, HP-UX, windows flavors, network administrators, database administrators , security administrators should redefine their job role themselves
This starts with introspection and will end at educating, equipping themselves with needed skills to project themselves class apart, stand ahead of the crowd even before the project requirement comes into picture. If we closely look at the reason behind the enterprise architectural changes starting 2017 most or all of these established firms, mid sized companies, startups all are looking for one single solution to sustain their business – CUT COST SAVE MONEY
This starts with migration of their unimportant applications, projects, environments onto cloud to make sure this does work fine and eventually retire the humongous servers, save cost on data center space, utility bills, server maintenance and at the end the firm does not need system administrator as the system is migrated out to cloud. The major job profession that will be impacted is system administration mainly Linux system administration job role. But this is the only one profession that does come with unique advantage of knowledge and experience of Linux making them referred choice of cloud administration. Let us look at the positive side of it. second much impacted profession is going to be DBA’s. Once a database is migrated onto cloud as relational data service RDS as they call it in AWS RDS, migration onto amazon aurora the primary market AWS is aiming for by providing data migration tool that makes migration easy using GUI, wherein all the database objects can be validated while migration is tested, AWS aims at making oracle database to amazon aurora migration possible as a piece of cake. This does apply to mysql which is again owned by oracle corporation. Coming to the oracle, mysql dba job threat not everyone will be laid off, but atleast half of the team can be eliminated as much of the administration is 100% automated at cloud level. So, oracle DBA should again start looking at positive side of it to see how they can equip themselves with needed skills for sustenance of their jobs
Why AWS when there are lot of cloud solutions?
I’ve analysed AWS, azure and found AWS as the preferred choice myself. Opinion differs and if your company is planning to migrate to azure you can think in those lines as well. Now coming to AWs, this firm has been in existence for past 10+ years from 2006 onwards. More than a decade existence has made AWS stable, robust platform with ton lots of options to choose from. Literally we can migrate the entire infrastructure onto AWS utilizing their services. To start with learn from scratch the architecture of AWS, different services that make it possible
We are creating ton lots of post to help our visitors learn AWs easy and simple, grow in their career. Keep supporting us


\1) What is the difference between primary key and unique key?
Primary key uniquely identifies a row. Unique keys are created in columns that will the unique row values. Primary key is unique and not null however unique key can have null values
\2) Why are you considering AWS while you have current job as DBA?
This is a very common interpersonal question. You can answer whatever you think of as the answer. But provide an answer that discusses advantage of cloud over on-perm systems. Also, mention that databases in future will be 100% hosted in cloud
\3) Why AWS instead of oracle cloud or azure environment?
If your current database profile is oracle DBA, SQL Server DBA the companies that have designed, developed, marketed your databases have their properitor platform for hosting the databases in cloud. To choose AWS over the other vendors major reason is that AWS is a decade old firm , growing extremely fast, stable that is much needed for sustainability of enterprise businesses. They cant choose a vendor for price reasons and waste money on migration projects later
\4) What is cloud computing?
This is a very common question that will be part of not only cloud dba but also other cloud support roles. Cloud computing in plain terms is migration of your data center to be taken care of by Amazon
\5) What are the many different AWS services supporting databases?
AWS RDS the relational database service supports many databases like mysql, postgresql, oracle, sql server and many more. Amazon dynamodb is popular nosql database. Amazon aurora comes in mysql as well as postgressql flavors that is developed, currently heavily marketed by amazon
\6) What is DMS?
The data migration service is a GUI from amazon that supports migration of current databases onto AWS cloud Aurora database. Interestingly feasibility , problems that could be encountered during migration including packages, objects that could be impacted post-upgrade will be listed while making use of DMS. This tool is used for migration of databases
AWS interview questions and answers
——————————————-
\1) Which AWS storage is used for long term data storage and archival? How sensitive information can be securely stored in this service?
Glacier is the long term archival storage used for data backup and archival on cost efficient basis. AWS glacier is a longterm data archival solution. Amazon Glacier is an extremely low-cost storage service that provides service as low as $0.004 per gigabyte per month also keeping it secure, durable, and flexible storage for data backup and archival. Glacier vault lock can be used to store information that are compliance sensitive and needs to be stored securely. In glacier with vault lock feature the regulatory and compliance data can be stored in immutable format as this data is write once read many called WORM format. Technically information stored in glacier is 99.99% durable. This is possible by storing data in multiple facility and multiple devices within each facility. In addition to all the advantages mentioned above this is least expensive option to store data meeting the requirements
\2) Can AWS glacier be used for CDN?
Nope. AWS is long term archival and backup solution and this is not CDN from AWS
\3) Is there a restriction on DNS naming convention on this amazon S3 bucket name in US regions?
All bucket names comply with DNS naming conventions. These conventions are enforced in all regions except for the US East (North Virginia) region
\4) Give details on reselling reserved instances in a EC2 environment :-
Reserved instances is the term given to the discount package that comes as part of general EC2 instance saving discount option. This discount can be availed by paying all upfront, partial upfront , no upfront cost. This reserves computing capacity for an EC2 instance from 1 year or 3 years. There is an option to resell the reserved instances in case of migration of EC2 instance to different availability zone, unexpected project termination, project completion before anticipated date. This will help you save money
\5) Give details on amazon S3 bucket versioning :-
We can enable S3 versioning that retained older version of missing files in AWS. In S3 bucket once we enable versioning it is like retaining many copies of same file. It is true that versioning will consume space but can be a savior in times of critical projects. In S3 versioning once enabled can’t be disabled. Only buckets can be copied and original buckets can be deleted. We need to copy the existing bucket to new bucket without versioning
\6) What is the use of copy-image command?
The command copy-image is used to copy an AMI from a specified source region to the current region. During copy we need to specify the destination region by using its endpoint when making the request
\7) What is the use of amazon resource name ARN’s?
Amazon Resource Names called as ARN’s uniquely identify AWS resources. An ARN is required when we need to specify a resource unambiguously across all of AWS, such as in IAM policies, Amazon Relational Database Service tags, and API calls
\8) What are the relational and non-relational databases included in amazon RDS services?
AWS Relational database service RDS includes relational database services like oracle, mysql, sql server, DynamoDB is the non-relational NoSQL database
\9) You have created a new security group. Does this allow all outbound traffic by default?
Yes, it does. By default, a security group includes an outbound rule that allows all outbound traffic
\10) In AWS RDS environment MySQL installations default to what port number?
In a typical mysql implementation 3306 is the default port. This should be secured safe and should not be accessible by untrusted hosts
\11) What is the advantage of using SWF instead of SQS in an order processing workflow in an ecommerce project?
An SWF workflow action is executed only once and hence the order processing needs to be using SWF instead of SQS to make sure the order processing does not repeat multiple times
\12) Is an AWS platform certified to use PCI DSS Level 1 ?
The Payment Card Industry Data Security Standard (also known as PCI DSS) is a proprietary information security standard administered by the PCI Security Standards Council, which was founded by American Express, Discover Financial Services, JCB International, MasterCard Worldwide and Visa Inc.PCI DSS applies to all entities that store, process or transmit cardholder data (CHD) and/or sensitive authentication data (SAD) including merchants, processors, acquirers, issuers, and service providers. The PCI DSS is mandated by the card brands and administered by the Payment Card Industry Security Standards Council.AWS has been PCI DSS Certified since 2010. As of July 11, 2016, an external Qualified Security Assessor Company (QSAC), Coalfire Systems Inc. has validated that Amazon Web Services (AWS) successfully completed PCI Data Security Standards 3.2 Level 1 Service Provider assessment and were found to be compliant for all the services outlined below.
Service provider levels are defined as:
Level 1: Any service provider that stores, processes and/or transmits over 300,000 transactions annually
Level 2: Any service provider that stores, processes and/or transmits less than 300,000 transactions annually
\13) What kind of storage is amazon S3?
Amazon S3 is an object based storage. In simple terms an amazon S3 creates buckets and the information is stored in buckets as objects
\14) You are moving data from amazon S3 to EC2 in the same region. How much do you need to pay for this?
We dont need to pay any money as there is no cost associated with moving data from S3 to EC2 in the same region
\15) For denying root access to EC2 instances can you make use of IAM policies that utilizes least privilege concept to restrict access via role assignment?
Root user is the super user in the system and has access to entire system including all of its resources and services. This can’t be restricted using IAM policies
\16) How will you protect a bastion host ?
A bastion host sits in a public subnet serving as secure gateway to SSH onto instance via private subnet
\17) Which AWS S3 solution will you recommend to store non-critical and reproducible data that needs to be stored with cost efficiency?
S3 reduced redundancy storage RRS can be used for cost efficient purpose
\18) Whish AWS service is ideal for BI tools and datawarehousing?
Redshift is datawarehouse, BI, big data solution from AWS
\19) Which amazon S3 resource stores data as objects?
While we start using amazon S3 to store files the first thing to do would be to creates AWS S3 buckets. This is the resource used to store data in the form of objects. In plain terms, once you upload your simple notepad file onto S3 it is stored in AWS s3 bucket as bucket object
\20) When a file of size 20GB is uploaded the error message: “Your proposed upload exceeds the maximum allowed object size.” is returned. What solution to this problem does AWS recommend?
In AWS S3 Multipart upload allows you to upload a single object as a set of parts. Each part is a contiguous portion of the object’s data. We need to design our application to use the Multipart Upload API for all objects
\21) Your environment has set of terminated instances. You have issued reboot-instances command. Should you be bothered about restart of terminated instances?
No need. Requests to reboot terminated instances are ignored while making use of reboot-instances command
\22) What is the strategy to control access to your Amazon EC2 instances?
This is accomplished using EC2 Security Groups
\23) You have launched a data collection campaign that is to last for five days. Which AWS EC2 purchase option best suits your needs?
On-demand instances allow us to pay for compute capacity on hourly basis with an option to increase or decrease compute capacity and pay hourly rate for instance used
\24) Is AWS redshift used to store bigdata by major companies?
Major industries including media, healthcare, finance, pharmaceutical, entertainment make use of S3 for scaling the systems that support big data, analytics, transcoding, and archive applications. Amazon redshift is datawarehouse solution and should not be confused with storing of big data
\25) You have been asked to map amazon EBS to an amazon EC2 for AWS CloudFormation resources. What is used for reference?
Reference the logical IDs of both EC2 and EBS. While creating CloudFormation template JSON needs to be built with all required attributes. These attributes are logical Id’s of EBS storage columns and EC2 instances. AWS cloudformation template created a JSON file with Resources section that declares the AWS resources to include in stack including EC2, block store that can be amazon S3 bucket, EBS etc. Resources of same type can be declared together. All resources must be declared separately. The logical ID is alphanumeric and unique within the template
\26) What is the availability percentage supported by AWS S3?
AWS S3 achieves 99.999999999% durability utilizing redundant storage of data across multiple facilities and multiple devices
\27) What is the use of AWS load balancer component?
The load balancer component of ELB monitors the traffic and handle the requests that come in through the Internet. Load balancer component is for traffic monitoring, controller service component of ELB deals with monitoring and managing load balancers
\28) How will you integrate AWS IAM with on-premises LDAP?
SAML can be used for on-premise LDAP integration as well as federated SSO implementation. Use SAML Security Assertion Markup Language to enable single sign-on between AWS and LDAP
\29) You have been tasked with identifying an appropriate storage solution for a 500GB database that requires random I/O reads of greater than 130000 4kB IOPS. Which EC2 option will meet this requirement?
The I2 Instance Type offers High I/O Performance Via SSD the solid state devices that offers fastest access of data. Make use of I2 series with scheduled backup
\30) What is the maximum number of simple workflow aka SWF domains allowed in a typical AWS account?
Amazon simple workflow service offers an option to maintain total of 100 registered domains that can be both registered and deprecated
\31) IS root user same as power user?
No. They are different users with different set of privileges. root is the superuser with supreme privileges
\32) What causes the error in an AWS environment – you are not subscribed to this service?
Your AWS account might have expired. Check the sale receipt and subscribe back to get access
\33) As part of our hadoop project in AWS cloud you are looking for a web interface to manage the Hive metastore. Which tool can be used?
Hadoop user experience aka HUE can be used for this purpose
\34) Which AWS service will you make use of to co-ordinate tasks across distributed application components?
Make use of amazon simple workflow AWS SWF to co-ordinate tasks across distributed application components
\35) Is it possible to copy amazon machine image across regions?
Yes, it is possible. It is possible to copy AMI within as well as across AWS region. This is possible using AWS management console, AWS CLI or SDKs
\36) How will you boot this HVM AMI?
Boot HVM amazon machine image by executing the master boot record of the root block device of the image
\37) Does amazon S3 buckets in usa regions alone provide eventual consistency for overwrite PUTS and DELETES?
This is partially true. As per Amazon S3 documentation eventual consistency for overwrite PUTS and DELETES is available in all regions
\38) When deploying databases on your EC2 instances what is AWS recommendation for better performance?
In general SSD the solid state devices are the fastest and are utilized in high throughput environment like SAP, highly transactional environments like OLTP. This is preferred option over magnetic storage devices
\39) Give details on naked domain names :-
Domain name without www the world wide web extension is a naked domain. Naked domain is also called zone apex records
\40) You are making use of amazon elastic search for your analytics project. How can you achieve high availability?
High availability can be achieved using Zone awareness
\41) How will you enable multifactor authentication in an AWS environment?
For multifactor authentication make use of IAM
\42) Give some facts about IAM :-
Every user you create in the IAM systems starts with No Permissions. IAM can be used to enable multifactor authentication in an AWS environment
\43) What will the the permission of the users that you create in IAM systems are going to start with?
It starts with no permissions
\44) What is Amazon CloudFront request handling capacity?
Amazon CloudFront can handle data transfer requests at the rate 1000 requests per second
\45) What is DMS? What is its use in an AWS environment?
The data migration service is a GUI from amazon that supports migration of current databases onto AWS cloud Aurora database. Interestingly feasibility , problems that could be encountered during migration including packages, objects that could be impacted post-upgrade will be listed while making use of DMS. This tool is used for migration of databases
\46) What is the maximum visibility timeout in amazon simple queue service SQS?
Maximum visibility timeout for amazon SQS message is 12 hours
\47) What does ICMP protocol translate to?
ICMP translates to Internet Control Message Protocol
\48) You have to enable the Virtual multi-factor authentication. Which AWS cloud service will you make use of for this purpose?
For enabling virtual multi-factor authentication in an AWS environment Identity and access management the IAM service is to be used
\49) How will you monitor CPU utilization of an EC2 resource in AWS environment?
Make use of AWS cloudwatch for monitoring EC2 resource utilization including CPU, memory
\50) Does RDS AWS service have access to operating system ?
Nope. Services like EC2, opsworks, EMR does have access to underlying operating system not RDS
\51) What is an EC2 instance? Your web site is hosted on 5 EC2 instances in 5 regions around the globe with 1 EC2 instance per region. How could you configure your site to maintain site availability with minimum downtime if one of the 5 regions was to lose network connectivity for an extended period of time?
In plain terms it is the virtual machine environment that hosts your application in AWS cloud. To minimize downtime create a Route 53 Latency Based Routing Record Set that resolves to Elastic Load Balancers in each region and has the Evaluate Target Health flag set to true.
\2) What are the many different storage options available with AWS?
Storage in S3 the standard storage, most popular archival service glacier, Reduced Redundancy Storage RRS in AWS terms, Elastic block store EBS storage, S3 IA the S3 Infrequent Access storage
\3) What is use of EC2 Security Groups?
Security groups implemented at EC2 instance level provides security at both protocol and port access level working way similar to firewall. This controls incoming as well as outgoing traffic in an EC2 instance
\4) How durable are the files saved in S3?
They are 99.999999999% durable
\5) You want to own your own private network in AWS. How can you accomplish this?
This can be accomplished using virtual private cloud VPC
\6) Your project makes use of S3 buckets as storage container. Do you need to provision this across multiple availability zones?
No need as the S3 storage is accessible across multiple availability zones
\7) What is Ephemeral storage?
It is the Temporary/Non Persistent storage
\8) What is the use of batch-write-item in a Dynamodb environment?
The batch-write-item is used to put or delete multiple items in one or more tables in dynamodb
\9) You are involved in business continuity project. You are currently working on disaster recovery. Do you know what does RTO stand for in disaster recovery?
Recovery Time Objective the stipulates time limit within which system needs to be up and running in case of failure. In business critical financial banks it is as low as 15 minutes in some cases
\10) How does an AWS on-demand instance work?
Here is the way an AWS on-demand instance work :
a) Pay as you go model. Pay only for usage thus saving cost
b) You are charged per second based on hourly rate
c) There is no upfront cost for instances and this avoids extra cost associated with unused instances
\11) What is the difference between primary key and unique key?
Primary key uniquely identifies a row. Unique keys are created in columns that will the unique row values. Primary key is unique and not null however unique key can have null values
\12) You are working on project where your employer has decided to migrate one of their projects onto AWS. What is the first thing to do while creating a new company account?
Set up new account using company official email address
\13) Is a power user given access to users within IAM?
Power user is one who has access to all AWS services except the management of groups and users within IAM. Root user is the superuser account that finds privilege over and above the power user account
\14) What is the use of cloudformation init script?
The cfn-init is the helper script that reads template metadata from the AWS::CloudFormation::Init key and acts accordingly . The AWS::Cloudformation::init key includes metadata on amazon EC2 instance. Following are the uses of a cloudformation init script :
a) Fetch and parse metadata from AWS:cloudformation::init key
b) Install packages
c) Write files to disk
d) Enable/disable services
e) Start (or) stop services
\15) How will you accomplish extra capacity with additional CPU and RAM in EMR?
By adding more task nodes this can be accomplished in an EMR node
\16) Which API call is internally triggered during the process of creating Amazon Machine Image AMI?
The API RegisterImage gets triggered during this process
\17) What is the use of an compute optimized instance?
This is an instance that is designed to provide moderate baseline performance and the capability to burst to significantly higher performance as required by our workload
\18) Where are individualized instances provisioned?
Individualized instances are provisioned at Availability Zones
\19) Your project makes use of RRS. You have made a decision to expand business in multiple zones. Can RRS sustain this data requirement?
RRS is designed to sustain the loss of data at a single facility and hence can’t be used for this purpose
\20) What is the total volume of data and number of objects that can be stored in Amazon S3 bucket?
1TB is the size limit
\21) You want to delete multiple objects from S3. How can you accomplish that?
This can be achieved using Multi-Object Delete operation
\22) What is the requirement with versioning in S3 to enable cross-regional replication?
Versioning must be enabled in both source and target S3 buckets for cross-regional replication
\23) Is multifactor authentication mandatory to delete objects from a S3 bucket?
To delete objects from S3 buckets multifactor authentication is an optional feature and not mandatory
\24) What is the minimum size of an S3 object?
Create a file with simple touch command and this will be 0 bytes. Such files with as small as 0 bytes can be created in S3
\25) How does amazon Simple workflow SWF help users?
The simple workflow service is used for task management in AWS environment . The tasks can be synchronous as well as asynchronous tasks. Coordinate synchronous and asynchronous tasks using AWS SWF
\26) If an Amazon EBS volume is an additional partition and not the root volume can we detach it without stopping the instance?
Yes, although it may take some time. An EBS volume other than root volume can be detached from live running instance. AWS CLI commands can be used for this purpose as well
\27) Your project uses SQL Server RDS. What is the maximum size for a Microsoft SQL Server DB with SQL Server Express edition in AWS?
There are two different limits one that of the database 10GB in size, and that of the DB instance server storage 300GB in size. A DB server instance could quite easily host several DBs, or a DB and support files such as logs, dumps, and flat file backups. For express edition 10GB is used
\28) What does EBS stand for?
Elastic Block Store EBS is the storage volume that is associated with EC2 instance in an AWS environment
\29) Which is a document that provides a formal statement of one or more permissions?
It is the policy document
\30) You are making use of AWs simple queue service. How many message queues can you create in SQS?
There is no limit on the number of message queues that can be created in SQS and it is unlimited
\31) What are some default methods of ingesting content into Amazon S3?
Internet, VPN are some default data ingestion methods onto amazon S3
\32) Can you store access keys in an AMI?
Access keys should never be stored on an AMI
\33) What AWS technologies will you make use of to ease the database load?
RDS read replica, Elasticcache are some database load AWS technologies
\34) What is main benefit of using AWS SWF worflow?
AWS SWF workflow ensures that actions are executed only once
\35) What is used to build elastic, self-healing applications in AWS?
Autoscaling groups can be used for this purpose
\36) Which service is the global content delivery network CDN from AWS?
Cloudfront is the Content Delivery Network from AWS
\37) Does amazon S3 support website redirects?
Yes. It does support redirects
\38) What is the minimum time interval for cloudwatch?
The minimum time interval for cloudwatch is 1 minute
\39) You have to migrate amazon S3 objects to Amazon Glacier. How can you accomplish that?
S3 lifecycle transition policy can be used for this purpose
\40) Can you make use of your existing microsoft windows server licenses with amazon EC2 shared tenancy instance?
This existing license can be used with dedicated host and not AWS
\41) How will you implement single sign-on in an AWS environment?
In AWS we can implement single sign-on by integrating with existing active directory account
\42) You are making using of AWs simple queue service. How many message queues can you create in SQS?
There is no limited on the number of message queues that can be created in SQS and it is unlimited
\43) What are the different types of EMR nodes?
Core nodes, Task nodes
\44) What are some of the benefits of AWS organizations?
a) Centrally manage access policies for multiple AWS accounts
b) Automation of AWS account creation and management
c) Control access to AWS services
d) Enable consolidated billing across multiple aws accounts
\45) What is the reason behind Route53 naming convention?
The DNS Port is on Port 53 and Route53 is a DNS Service
\46) You want to get details on TTL in a specified table. Which command will you make use of?
describe-time-to-live can be used to get details on TTL
\47) Give some AWS services that have access to operating system :-
In AWS environment EC2, sysopswork are some services that have OS access
\48) In a ELB implementation which component of ELB does monitor the load balancers?
In ELB controller service monitors the load balancers. This includes tasks such as adding and removing load balancers as needed. The load balancers are verified for proper functionality and removed or added on as needed basis
\49) You are configuring encryption when creating the EBS volume. Does this enable encryption at rest ?
Yes. It does apply to both at rest and dynamic info
\50) Can you create placement groups across 2 or more availability zones?
Nope. It is not possible to do so
\51) What are all the payment options associated with reserved instances?
Following are the payment options associated with reserved instances:
a) All upfront
b) Partial upfront
c) No upfront
\52) Can ELB distribute traffic across regions?
Nope, not possible. ELB can distribute traffic across EC2 instances. The EC2 instances can be in same availability zone, different availability zone within same region. ELB does nto distribute traffic across regions
\53) You are looking for a robust delivery solution to transfer data from amazon lambda function onto amazon elastic search. Which service will you make use of?
AWS Kinesis firehose can be used for this purpose
\54) You have been asked to build a system to analyse the customer behaviour. The data used for analysis comes from many different data sources including sales report, tweets, customer order logs from database. How will you build the basic framework for this project?
This project implementation tarts with datalake
\55) What is the maximum length of the streamname string in amazon kinesis stream ?
The maximum length is 128
\56) Does Elastic Map Reduce allows you to access the underlying operating systems of the EMR nodes?
Yes, it does allow OS access
\57) Who is a owner in AWS permission model?
Both user identity and email address are used to create AWS account
\58) Does Route53 support MX the mail Records?
Yes. IT does support MX mail records
\59) What kind of data is stored in AWS glacier service?
AWS glacier is a data archival solution thatis mainly used to store Infrequently accessed data & data archives
\60) You have deleted your ELB. Do you know how long cloudwatch metrics data are accessible for deleted ELB?
It becomes accessible for a period of 2 weeks
\61) What are the many different types of actors in amazon simple workflow service?
Amazon SWF interacts with programmatic actors such as workflow starters, deciders, or activity workers
\62) What is the use of domain in amazon simple workflow service SWF?
a) workflow components including workflow types, activity types can be specified to be part of domain scoping the amazon SWF resources within the AWS account
b) Domain is a collection of related workflows
\63) Does AWS support SOAP?
SOAP support is available over https. It is not available over http also amazon s3 new features dont support SOAP
\64) What makes DynamoDB a suitable choice for gaming websites?
DynamoDB is a fast, fully managed NoSQL database service that makes it simple and cost-effective to store and retrieve any amount of data, and serve any level of request traffic. Its guaranteed throughput and single-digit millisecond latency make it a great fit for gaming, advertising technology, mobile, and many other applications
\65) Can we detach EBS volume that forms the root device of the EC2 instance without stopping the instance?
Nope, not possible. As in normal linux (or) unix machines root volume is the main volume that needs to be accessible for the machine to be up and running without any issues. Same does apply to EC2 instances as well
\66) Do you know how long cloudwatch metrics data are accessible for terminated AWS EC2 instance?
This information becomes available for a period of 2 weeks
\67) What is the VisibilityTimeout value of an SQS message in a FIFO queue?
The VisibilityTimeout is 12 hours
\68) Do you know which language is made use of while creating IAM policy documents?
JSON is used for this purpose
\69) You are looking for a easy way to load streaming data into AWS. Which service will you use?
Kinesis Firehose serves this purpose
\70) You are connecting to AWS using AWS CLI. What do you need for this?
For this do we need to create an IAM user
\71) Which operation in dynamodb lets you support atomic counters?
UpdateItem supports atomic counters
\72) We are creating an amazon S3 bucket from US standard region. Can I make it mixed case?
Nope. Amazon S3 buckets should be all lower case. This is across all AWS regions and not specific to Us standard region etc
\73) How can you accomplish amazon kinesis API to add tags to stream?
This can be accomplished using AddTagsToStream
\74) What AWS services can you make use of to gather requirements on your payments application development project in AWS?
Amazon payments infrastructure are made use of by services amazon devpay and amazon FPS. amazon flexible payment services is a service used by developers to accept payments on websites. this includes micropayments support as well. When it comes to amazon devpay the scope is different. Say you have applications built on amazon s3 or amazon ec2. You want to resell these applications, Now, the customers pay amazon. Amazon deducts a small fee plus commission and pays rest to you. This is tightly integrated with AWS infrastructure
\75) What is a EBS snapshot?
In Amazon EBS terms, EBS snapshot is state of a EBS volume captured at a point-in-time
\76) What are components of Elastic Load balancer ELB?
ELastic load balancer ELB as it is popularly called is composed of two components the load balancer and the controller services
\77) S3 has eventual consistency for which HTTP Methods?
AWS S3 provides eventual consistency for overwrite puts and deletes