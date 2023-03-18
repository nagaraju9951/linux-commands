

# File Commamds

    • ls : The command is used  for in listing contents inside a directory.



    • cat : The Cat commamd is frequently used command to display the data of the file
        Cat Filename.
        Cat file2 enter.



    • more:  The more command is used to view the text files in the same command
         create some
         files 1,2,3,4,5,6 more file{1..5}.


    • tail :  The tail command is used to display the last 10 lines or 10 files .
              tail file1

         .

    • tail -f : tail -f command can be used to monitor the growth of a file being written by another
            process .
           tail -f file1


    • locate : The locate command finds files in Linux using
    •   cd :  cd command is used to change the current working directory.
        cd .. - Change to the parent directory of the current working directory.
        cd ~ - Change to the home directory of the current user.
        cd / - Change to the root directory of the file system.


    •  mkdir : Create directory.
                  Mkdir python.



    • touch : create emty files.
             Touch file{1..5}.

    • move : The move is used to move one or more files or directories from one place to another.
             mv file1 file2



    • rm : rm command is used to delete the file
       Ex : rm -r file name.

    • rmdir : command is used to remove a directory. It is a simple and straightforward command that removes the specified empty directory.
        ex : rmdir directory.
    • Vi-Esc : The command moves the cursor from any position on that line. Press Esc to return to command mode after you type the desired text.
          Ex : Vi filename.

    • i: Switch to insert mode.
	 Ex : “ i “ enter

    • d : This Command is used to delete the command lines.

    • dd :  This command is also similar to ‘d’ This ‘dd’ command is used to delete the two lines
       	at  a time.

    • x : the "x" command deletes the character under the cursor. Press “esc” and click “x”.

    • xx : In insert mode, typing "xx" inserts the characters "xx" into the document at the current
        	cursor position .

    • q! : it is used to quit without saving changes.

    • wq! : it uses to save and quit .

    • cp :  copy the file or directories from one location to another location.

    • cp -r : copy files along with sub directoriesthe destination location.

    • sed : This command is used to edit files quikely and efficent.
       	 ‘s/1/2’ file1.


    • find – size : To find all files larger than a certain size
      	   find . - size +1mb.
    • Date : this command is used to show the date .
	  	Ex : Date enter.


    • grep : grep command filters the content of a file which makes our search easy .
    	  Ex : grep keyword filename grep calss 2 is [keyword] file2 is [filename].


    • Grep -i : grep -i command is used to perform a case-insensitive search.
             grep -i "example" filename .
             Ex : grep -i “hi” file2.

    • du : Du is is disk usage the du command is used to estimate file space usage.
	        Ex : [du filename] .


    • df : disk file  usage This will display the disk space usage for the file system
     	  that contains the specified directory.
	      Ex: df  -h /path/to/directory.

    • Diff : This command is used to find the difference between the file to file and
       	  directories to directories.
       	  Ex : diff file1 file2.


    • wc -l : This command in Linux is used to count the number of lines in a file.
            wc -l file2.


    • Tar : This command is used to create, manipulate, and extract files from tar archives.
           Ex : Create file tar -cf mytar_tar filename.
                Extrat tar -xvf archive.tar
                add tar -rvf achive.tar file1 file2
                compress tar – czvf achive.tar.gz file1 file2.

    • Zip : A zip archive is a collection of files that are compressed and combined into a single
            file for easy distribution or backup.
            Ex : create a new zip : zip archive.zip file1 file2 devops.
             extract the contents of a zip : unzip archive.zip.
             add files to an existing zip : zip -r archive.zip file3 devops2.
             compress a zip : zip -9 archive.zip file1 file2 devops 1

    • unzip :  used to extract files from a compressed zip archive.
             Ex : unzip archive.zip

    • ln : command is used to create links to files or directories.
            EX : In -s [target file] [symbolic filename].

# User Management

    • useradd : command to create a new user account.
	EX :
                 sudo useradd raju
                 sudo useradd mk
                 sudo useradd hk.
           user exist or not : cat /etc/passwd enter

    • passwd : This command is used to to change the password.
                Ex :   sudo passwd mk.
                       sudo passwd hk.

    • userdel :  to verify deletion is complete or not.
            Ex :    Sudo userdel mk
             sudo userdel hk.
# Access Management

    • ssh :  ssh is Secure Shell SSH protocol provides a secure channel between two devices.
             Ex : scp /path/to/local/file username@remote_host:/path/to/remote/directory.

    • scp : Linux is used to copy files securely between hosts on a network.
                                                                                                                                                                                      
            Ex : scp myfile.txt user@remotehost:/home/user.

    • Sudo : it is a command superuser do.
    	`  Ex : sudo command_to_execute.

    • su : it is command used to allows a user to switch to another user account or becomes the super account or root user.
              Ex :      nagaraju@nagaraju:~$ sudo su
                        [sudo] password for nagaraju:
                        root@nagaraju:/home/nagaraju# ^C
                        root@nagaraju:/home/nagaraju# .

    • Chmod : it is a command to change the permissions of files and directories.
	        Ex : chmod 777 pythonfile1 .

    • Chown : it is a command is used to change the owner .
	       Ex : chown mk file1.

 # Configuration Management.

    • env : it is a environment change.
	     Ex : env |more.

    • path : list if directories saperated by colons.
	      Ex echo $path

    • Echo : it is used to display text on the terminal.
	    Ex : echo "hi hello ".

    • Expoet : it is used to set environment varables.
  	  Ex : export google
  	      echo google.

    • Hostname : it is used to get or set hostname.
	  Ex : hostname.

    • Netstat : this command is used to display the network connections and network statistcs of the system.
	   Ex : netstat enter.

    • crontab - l : to view the corntab.

    •    corntab -L which is used to schedule the job.
	    Ex :
	        root@nagaraju:~# cd devops
	        root@nagaraju:~/devops# crontab -l
	        no crontab for root
	        root@nagaraju:~/devops# crontab -e
	        no crontab for root - using an empty one
	        crontab: installing new crontab
	        root@nagaraju:~/devops# crontab -l
	        * * * * * /home/root/test.sh
	        root@nagaraju:~/devops#

    • Kill : command is used to process send a signal to a processer to terminate it
	       Ex : kill 1234 .
    • P kill : To terminate all processes with a specific name, using the pkill command.
	        Ex : pkill firebox.

    • wget : it is command used to download files from internet.
	        ex :    root@nagaraju:~/devops# cd
	root@nagaraju:~# wget https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.7/bin/apache-	tomcat-10.1.7.tar.gz
                --2023-03-07 17:21:47--  https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.7/bin/apache-		tomcat-10.1.7.tar.gz
                Resolving dlcdn.apache.org (dlcdn.apache.org)... 2a04:4e42::644, 151.101.2.132
                Connecting to dlcdn.apache.org (dlcdn.apache.org)|2a04:4e42::644|:443... connected.
                HTTP request sent, awaiting response... 200 OK
                Length: 12143798 (12M) [application/x-gzip]
                Saving to: ‘apache-tomcat-10.1.7.tar.gz’

                apache-tomcat-10.1.7.tar.gz                        100%[===============================================================================================================>]  

                2023-03-07 17:21:48 (9.93 MB/s) - ‘apache-tomcat-10.1.7.tar.gz’ saved [12143798/12143798]

                root@nagaraju:~# ^C
                root@nagaraju:~# .

    • curl : it is command is used to transfer the fies.
	  Ex : curl -V.

    • ping : command is used to test the connectivity between two networks.
	     Ex : ping google.com.

    • uname : to display the user Name.
	     Ex Uname.

    • Histiry : is used to show the history.
        Ex : history.

    •   ps ux : command that displays a list of all process running in the system, including their associate user and cpu/memory usage.
	   Ex : pu us.root@nagaraju:~# ps ux
	USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
	root           1  0.0  0.1 169652 12696 ?        Ss   07:07   0:05 /sbin/init splash
	root           2  0.0  0.0      0     0 ?        S    07:07   0:00 [kthreadd]
	root           3  0.0  0.0      0     0 ?        I<   07:07   0:00 [rcu_gp]
	
    • ps -ef|grep <pid> : used to for finding information about a specific process running in the 	linux system.
	 Ex:    root@nagaraju:~# ps -ef|grep devops
	        root       28669   22958  0 17:44 pts/0    00:00:00 grep --color=auto devops
        root@nagaraju:~# .

# Log Management 

    • syslog : To view the entire systemlog.
             Ex : cd devops
                     cat /vat/log .

    • journalctl : is a powerful tool for working with system logs and troubleshooting issues in Linux operating systems.
	Ex :  journalctl.
	        journalctl -S "2023-03-01 00:00:00" -U "2023-03-07 23:59:59" .

    • costom logs : In Linux, you can create custom log files using the logger command or by redirecting output to a file.

 # Network Management

    • Ifconfig : displays information about all network interfaces on the system, including their IP      address, netmask, and hardware address (MAC address). 

    • Http : HTTP Hypertext Transfer Protoco is not secure. 
	 Ex : http://www.google.com .

    • Https : HTTPS Hypertext Transfer Protocol Secure it is secure.
	Ex : https://www.google.com .
	 internal network : An internal network is a private network that is restricted to a specific 	organization or group of users .
	Ex : This can be done by Ifconfig .
    • External network : an external network refers to a network that is outside of your local network or organization.
	Ex : ping google.com
    • TCP : Transmission Control Protocol is a connection-oriented protocol that provides reliable, ordered, and error-checked delivery of data between applications running on hosts on a network. 
	 Ex : Facebook , Snapchat.

    • UDP  : udp stands for User Datagram Protocol. UDP sends small packets of data, called datagrams, to the receiving host without waiting for an acknowledgement of receipt. This allows for faster transmission of data, but also means that packets may be lost or arrive out of order.
	Ex : skype ,zoom, jiomeet, web x meet.

    • Private Subnets : Private subnets are a range of IP addresses that are reserved for use within private networks, such as local area networks .
	 Ex : 10.0.0.0/8: This includes all IP addresses from 10.0.0.0 to 10.255.255.255 this addres 	for      	private use.
    • Public subnet : They are used to host resources that need to be accessible from the Internet, such as web servers, email servers, and application servers. Public subnets are typically associated with a public IP address, which allows incoming traffic from the Internet to reach the resources hosted within the subnet.
    • CIDR Range Calculations : CIDR (Classless Inter-Domain Routing) is a method for allocating IP addresses and defining network prefixes. CIDR notation represents an IP address and its associated network prefix as a single value, such as 192.168.1.0/24.

    • Port : port is a logical channel through which network communication is established between two processes on different machines. Each port is associated with a unique number between 0 and 65535. 
		Ex :  Port 22 .

    • Application : a software program designed to perform a specific function or set of functions. 
		Ex : apache tomcat server ,microsoft ias , jboss eap

    • Web servers  : A web server is a software application that serves web pages over the Internet.
		Ex : apache HTTP server, Nginx Caddy.

    • Load balancing  : is the process of distributing incoming network traffic across multiple servers to ensure high availability and performance.
	Ex : round robin 
	least connection 
	Ip Hash 
	Weighted round robin
	Least response time.
 

    • HA : High Availabilit , which is a system design approach that aims to ensure a high level of system availability and reliability by minimizing downtime and providing failover capabilities.
	 Several tools are used in Ha 
		Ex : HAProxy ,Corosync .

# AWS Devops


 08/04/2023

66.  ls
67.  ls -ltr
68. ssh -i"demo-ec2.pem" ubuntu@50.18.85.216
69.  chmod 400 demo
70.  chmod 400 demo-ec2.pem
71.  cd ~/Downloads/demo/
72.  chmod 400 demo-ec2.pem
73.  cd ..
74. git clone https://github.com/nagaraju9951/Linux-comands-Update.git
75.  ls
76.  ssh -i "demo-ec2.pem" ubuntu@50.18.85.216
77.  ls
78.  ssh -i "demo-ec2.pem" ubuntu@50.18.85.216
79.  chmod 400 demo-ec2.pem
80.  ssh -i "demo-ec2.pem" ubuntu@50.18.85.216
81.  scp -i "demo-ec2.pem" -r linux-commands-updates ubuntu@50.18.85.216:/home/ubuntu/mk
82.  scp -i "demo-ec2.pem" -r  ubuntu@50.18.85.216:/home/ubuntu/
83.  Linux-comands-Update
84.  scp -i "demo-ec2.pem" -r 
85.  Linux-comands-Update
86.  scp -i "demo-ec2.pem" -r Linux-commands-Update ubuntu@50.18.85.216:/home/ubuntu/mk
87.  scp -i "demo-ec2.pem" -r Linux-comands-Update ubuntu@50.18.85.216:/home/ubuntu/mk
88.  ssh -i "demo-ec2.pem" ubuntu@50.18.85.216
89.  asss
90.  exit
91.  ssh -i"demo-ec2.pem" ec2-user@13.56.79.16
92.  ssh - i demo-ec2.pem ec2-user@13.56.79.16
93.  ssh -i "demo-ec2.pem" ec2-user@13.56.79.16
94.  ls -ltr
95.  ssh -i "demo-ec2.pem ec2-user@172.31.19.29
96.  ssh -i "demo-ec2.pem" ec2-user@172.31.19.29
97.  ssh -i "demo-ec2.pem ec2-user@172.31.19.29
98.  ssh -i "demo-ec2.pem" ec2-user@13.56.79.16
99.  ssh -i "demo-ec2.pem ec2-user@172.31.19.29
100.  ssh -i "demo-ec2.pem" ec2-user@13.56.79.16
101. ls -ltr
102.  ssh -i demo-ec2.pem ec2-user@13.56.79.16
103.  history
104.  clear
105.  ls
106.  ll -ls
107.  ssh -i "demo-ec2.pem" ubuntu@18.144.75.55
108.  chmod 400 demo-ec2.pem
109.  chmod 400 "demo-ec2.pem"
110.  git clone https://github.com/nagaraju9951/Linux-comands-Update.git
111 . ls
112.  chmod 400 demo-ec2.pem
113.  chmod 400 "demo-ec2.pem"
114.  ls -ltr
115.  ssh -i "demo-ec2.pem" ubuntu@13.52.213.151
116.  cd
117.  history

09/04/2023

115.  ssh -i "demo-ec2.pem" ubuntu@13.52.213.151
116.  cd
117.  history
118.  clear
119.  ls
120.  cd Download
121.  cd Downloads
122.  ls
123.  ssh -i "demo-ec2.pem" ubuntu@54.219.176.180
124.  scp -rp "demo-ec2.pem" ubuntu@54.219.176.180:/home/ubuntu/dell
125.  scp -rp Linux-comands-Update ec2-user@54.241.109.221:/home/ubuntu/dell
126.  scp -rp Linux-comands-Update ubuntu@54.241.109.221:/home/ubuntu/dell
127. 
128.  scp -rp "demo-ec2.pem" ubuntu@54.219.176.180:/home/ubuntu/dell
129.  scp -rp Linux-comands-Update ubuntu@54.219.176.180:/home/ubuntu/dell
130.  ls
131.  ssh -i "demo-ec2.pem" ec2-user@54.241.109.221
132.  ssh -i "demo-ec2.pem" ubuntu@54.241.109.221
133.  scp -rp "demo-ec2.pem" ubuntu@54.241.109.221:/home/ubuntu/dell
134.  scp -rp "demo-ec2.pem" ubuntu@54.241.109.221:/home/ubuntu/dell1
135.  scp -rp demo-ec2.pem ubuntu@54.241.109.221:/home/ubuntu/dell1
136.  scp -rp "demo-ec2.pem" ubuntu@54.241.109.221:/home/ubuntu/dell1
137.  scp -rp Linux-comands-Update ubuntu@54.241.109.221:/home/ubuntu/dell1
138.  history 


12/04/2023
ls
642.  ls -l
643.  cd Downloads/
644.  ls -l
645.  chmod "jumphostkey.pem"
646.  chmod 400 "jumphostkey.pem"
647.  ls -l
648.  chmod 400 "demokey.pem"
649.  ls -l
650.  cd .ssh
651.  exit
652.  ls -l
653.  cd .ssh
654.  ls
655.  vi config
656.  ssh demohost
657.  jumphost
658.  cd
659.  cd Downloads/
660.  ls l
661.  ls -l
662.  cd
663.  cd .ssh
664.  vi config
665.  ssh demohost
666.  ssh jumphost
667.  ls
668.  cat config
669.  vi config 
670.  ssh demohost 
671.  cat /home/nagaraju/Downloads/demokey.pem
672.  cat /home/nagaraju/Downloads/jumphostkey.pem
673.  ls
674.  vi config 
675.  ssh demohost 
676.  ssh jumphost
677.  cd

# personal AWS account
   A personal AWS (Amazon Web Services) account is a type of account that an individual can create to access and use various cloud computing services  	    offered by Amazon through AWS. These services include computing, storage, databWhen you create a KMS key, AWS generates a unique cryptographic key #KMS(Encryption) Keys
   key management servicethe is used to encrypt and decrypt your data. You can then use this key to encrypt your data before storing it in an AWS 		service, and decrypt it when you need to retrieve it.ase, analytics, and other related services.Security Groups
# Security Groups
  Security Groups can be thought of as a set of rules that define what traffic is allowed to enter or leave a specific resource. For example, you can       create a Security Group that allows inbound SSH traffic on port 22, or outbound HTTP traffic on port 80.
  Ex : 1 default security
       2 custom security.
    
# SSH keys in AWS.
   Shh is Secure Shell is a network protocol used to securely connect to and manage remote servers or instances in a virtual private cloud (VPC) in AWS.    It provides a secure way to access and manage your EC2 (Elastic Compute Cloud) instances, without exposing them to the public internet.
   
 # Create an Encryption key with KMS in Aws
    KMS is Key Management Service KMS is a fully managed service that makes it easy for you to create, control, and manage encryption keys used to secure     your data. 
    steps to create KMS
    1.Open the AWS Management Console and navigate to the KMS service.
    2.Click on "Create key" and select the type of key you want to create. You can choose either symmetric or asymmetric encryption.
    3.Set the key details, such as the alias, description, and key usage permissions.
    4.Configure the key policy to specify who can use the key and what actions they can perform.
    5.Review and confirm the settings, and then create the key.
    
 # Create security Groups in Aws
        1 .Open the AWS Management Console and navigate to the EC2 (Elastic Compute Cloud) service.

	2 .Click on "Security Groups" in the left-hand navigation pane.

	3 .Click on the "Create Security Group" button.

	4 .Enter a name and description for the Security Group.

	5 .Choose the VPC (Virtual Private Cloud) for which the Security Group will apply.

	6 .Add inbound and outbound rules to the Security Group.
	These rules specify the type of traffic that is allowed or denied in the Security Group. For example, 
	you can allow inbound SSH traffic on port 22 from a specific IP address or range.

	7 .Review the Security Group settings and click on "Create Security Group".
	
# create ssh key in aws
   The key pair consists of a public key and a private key, and it allows for secure and encrypted communication between the client (your computer) and      the server.
   steps to create ssh keys
1. Open the AWS Management Console and navigate to the EC2 (Elastic Compute Cloud) service.
2. Click on "Key Pairs" in the left-hand navigation pane.
3. Click on the "Create Key Pair" button.

4. Enter a name for the key pair in the "Key pair name" field.

5. Select "SSH-2" as the key pair type.

6. Click on the "Create Key Pair" button.

7. The private key file will be downloaded automatically. Save this file in a secure location on your computer.

8. The public key will be displayed in the console. Copy the public key to use when connecting to your EC2 instances.
	
# Open only necessary ports in the Security Group


1. Open the AWS Management Console and navigate to the EC2 (Elastic Compute Cloud) service.

2. Click on "Security Groups" in the left-hand navigation pane.

3. Select the Security Group you want to modify and click on the "Inbound Rules" tab.

4. Click on the "Edit" button.

5. Modify the inbound rules to allow only necessary ports.

6. Remove any existing rules that are not necessary.

7. Click on the "Save Rules" button to apply the changes.
	
#EC2 Instances
  EC2 instances can be used for a variety of purposes, such as hosting websites, running applications, 
  performing data processing and analysis.
  
#instances types
1. General purpose
2. Compute optimized
3. Memory optimized
\4. Storage optimized
#Volumes in Aws
1. Sign in to the AWS Management Console and navigate to the EC2 dashboard.
2. Click on "Volumes" in the left-hand menu.
3. Click on the "Create Volume" button.
4. Specify the volume settings, such as volume type, size, availability zone, etc.
5. Click on the "Create" button to create the volume.
Once the volume is created, you can attach it to an EC2 instance or keep it as a separate volume for storage.

# Amis 
Amazon provides a variety of public AMIs that users can choose from, or users can 	create their own custom AMIs based on their specific requirements. AMIs can also be 	shared between users or kept private for personal use.

# snapshots 
a snapshots takes a copy of EBS volume and place it in Amzon s3 ,
where it is stored redundantly in multiple Avalibility zones. 
snapshots are a useful tool for creating backups, 
testing new configurations, and recovering from failures or other issues.

# EC2 Instances menu
1.instance : instance is nothing but the Instances in AWS can be created from pre-configured Amazon Machine Images (AMIs) that contain an operating system and any additional software or configuration that is required for the application. 
Instances can be launched, stopped, started, and terminated as needed, providing flexibility in managing computing resources in the cloud.

2.Instance types in aws ec2 : There are a wide variety of instance types available in AWS, each with its own set of specifications and features.
  -- types of instances
  a.General-purpose instances
  b.Compute-optimized instances
  c.Memory-optimized instances
  d.Storage-optimized instances 
  
#Launch template 
Launch Templates allow you to specify various parameters for EC2 instances,
such as instance type, storage, security groups, network settings, and more. 
By defining these settings in a Launch Template, you can quickly and easily launch multiple instances with consistent configurations and settings.

# sopt request
1. Spot Requests allow you to take advantage of unused EC2 capacity in the AWS cloud, which can help reduce your EC2 costs.
2. Spot instances are ideal for workloads that are flexible in terms of when they can be run, such as batch jobs, background processing, and               development/testing environments.

 first open cloud9 in search box

# Create a snapshot from the root volume of the above instance and create a custom AMI
from the snapshot.
 Stemps for snapshort : 
	1. go instace select it
	2. select volume and select the volume and click actions and create snap
	3. select snap and
	4. press CLOUD WATCH in seacrch box and select rules.
	5 . give details which has appeared on screen.
# Create EC2 Instance from the Custom AMI.
1. Go to the AWS Management Console and navigate to the EC2 service.
2. Click on "Launch Instance" button to create a new instance.
3. In the "Choose an Amazon Machine Image (AMI)" step, select "My AMIs".
4. Select the custom AMI you want to use to launch the instance.
5. Choose an instance type based on your requirements.
6. Configure the instance details, such as VPC, subnet, security group, and key pair.
7. Review the instance details and click on the "Launch" button.
8. If you selected an existing key pair during instance configuration, download the private key (.pem) file and store it in a safe place. If you did not 9 .select an existing key pair, create and download a new key pair.
10. Wait for the instance to launch. Once it is launched, you can connect to it using SSH or Remote Desktop depending on the operating system of the   		instance.
After connecting to the instance, you can customize it as per your requirements.

# Configure local .ssh/config to connect to remote EC2 instances.
115.  ssh -i "demo-ec2.pem" ubuntu@13.52.213.151
116.  cd
119.  ls
120.  cd Download
121.  cd Downloads
122.  ls
123.  ssh -i "demo-ec2.pem" ubuntu@54.219.176.180
124.  scp -rp "demo-ec2.pem" ubuntu@54.219.176.180:/home/ubuntu/dell
126.  scp -rp Linux-comands-Update ubuntu@54.241.109.221:/home/ubuntu/dell
129.  scp -rp Linux-comands-Update ubuntu@54.219.176.180:/home/ubuntu/dell
130.  ls
131.  ssh -i "demo-ec2.pem" ec2-user@54.241.109.221
138.  history 

# NACL 
NACL helps in providing a firewall there by helping secure the VPCs and subnets. 
It helps provide a security layer which controls and efficiently manages the traffic that moves around in the subnets. 
It is an optional layer for VPC, which adds another security layer to the Amazon service. 

# s3 Bucket
 s3 : amazon simple storage service
 S3 provides a simple web services interface that enables you to store and retrieve any amount of data from anywhere on the web. 
 stemps to create s3 bucket
1. search bar search s3
2. Click on the "Create Bucket" button.
3. Enter a unique and descriptive name for your bucket.
4. Select the region in which you want to create the bucket.
5. Choose the appropriate settings for the properties, such as versioning and encryption, based on your needs.
6. Set the permissions for your bucket, including access control policies and permissions.
Review your settings and click "Create Bucket" to create your S3 bucket.

# ELB
It helps improve the availability, scalability, and reliability of applications by distributing traffic
across multiple targets and automatically routing traffic to healthy targets in the event of a target failure.

# target group
Target Groups can be used with both Application Load Balancers (ALB) and Network Load Balancers (NLB). 
When a request is received by the load balancer, it is routed to a specific Target Group based on the rules and conditions defined in the load balancer. The Target Group then routes the request to a set of targets that meet the criteria specified in the Target Group configuration.




