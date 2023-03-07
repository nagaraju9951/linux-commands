
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

i: Switch to insert mode.

d : This Command is used to delete the command lines.

dd :  This command is also similar to ‘d’ This ‘dd’ command is used to delete the two lines   
       at  a time.

x : the "x" command deletes the character under the cursor. Press “esc” and click “x”.

xx : In insert mode, typing "xx" inserts the characters "xx" into the document at the current
        cursor position .

q! : it is used to quit without saving changes.

wq! : it uses to save and quit .

cp :  copy the file or directories from one location to another location.

cp -r : copy files along with sub directoriesthe destination location.

sed : This command is used to edit files quikely and efficent.
	"s/1/2" file1.


find – size : To find all files larger than a certain size 
         find . - size +1mb.


Date : this command is used to show the date .
  Ex : Date enter.


grep : grep command filters the content of a file which makes our search easy . 
      Ex : grep keyword filename grep calss 2 is [keyword] file2 is [filename].


Grep -i : grep -i command is used to perform a case-insensitive search.
             grep -i "example" filename . 
	     Ex : grep -i “hi” file2.
  
du : Du is is disk usage the du command is used to estimate file space usage.
	Ex : [du filename] .

       
df : disk file  usage This will display the disk space usage for the file system  
       that contains the specified directory. 
      Ex: df  -h /path/to/directory.

       

Diff : This command is used to find the difference between the file to file and 
         directories to directories.  
         Ex : diff file1 file2.




wc -l : This command in Linux is used to count the number of lines in a file.
          wc -l file2.

          
Tar : This command is used to create, manipulate, and extract files from tar archives. 
           Ex : Create file tar -cf mytar_tar filename.
                Extrat tar -xvf archive.tar 
                add tar -rvf achive.tar file1 file2
                compress tar – czvf achive.tar.gz file1 file2.

Zip : A zip archive is a collection of files that are compressed and combined into a single
         file for easy distribution or backup.
        Ex : create a new zip : zip archive.zip file1 file2 devops.
             extract the contents of a zip : unzip archive.zip.
             add files to an existing zip : zip -r archive.zip file3 devops2.
             compress a zip : zip -9 archive.zip file1 file2 devops 1

unzip :  used to extract files from a compressed zip archive.
             Ex : unzip archive.zip

ln : command is used to create links to files or directories.
  EX : In -s [target file] [symbolic filename].
  
# User Management

useradd : command to create a new user account.
EX :
                 sudo useradd raju 
		 sudo useradd mk
		 sudo useradd hk.
user exist or not : cat /etc/passwd enter
                 
passwd : This command is used to delete the existing user.
  	Ex :    sudo passwd mk.
		sudo passwd hk.

userdel :  to verify deletion is complete or not.
     Ex :    Sudo userdel mk
	     sudo userdel hk.
# Access Management
 
 ssh :  ssh is Secure Shell SSH protocol provides a secure channel between two devices.
	Ex : scp /path/to/local/file username@remote_host:/path/to/remote/directory.
	
scp : Linux is used to copy files securely between hosts on a network.
  Ex : scp myfile.txt user@remotehost:/home/user.
 
 Sudo : it is a command superuser do.
  Ex : sudo command_to_execute.
  
su : it is command used to allows a user to switch to another user account or becomes the super account or root user.
	      Ex :      nagaraju@nagaraju:~$ sudo su
			[sudo] password for nagaraju: 
			root@nagaraju:/home/nagaraju# ^C
			root@nagaraju:/home/nagaraju# .

Chmod : it is a command to change the permissions of files and directories.
 	Ex : chmod 777 pythonfile1 .
	
Chown : it is a command is used to change the owner .
       Ex : chown mk file1.
       
 # Configuration Management.
 
 env : it is a environment change.
     Ex : env |more.
    
   path : list if directories saperated by colons.
      Ex echo $path
      
   Echo : it is used to display text on the terminal.
    Ex : echo "hi hello ".
    
    Expoet : it is used to set environment varables.
    Ex : export google
    	echo google.
	
Hostname : it is used to get or set hostname.
  Ex : hostname.
 
 Netstat : this command is used to display the network connections and network statistcs of the system.
   Ex : netstat enter.
   
   crontab - l : to view the corntab.
   
   corntab -L which is used to schedule the job.
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

Kill : command is used to process send a signal to a processer to terminate it
       Ex : kill 1234 .
      
 P kill : To terminate all processes with a specific name, using the pkill command.
  	Ex : pkill firebox.
	
wget : it is command used to download files from internet.
	ex :	root@nagaraju:~/devops# cd
		root@nagaraju:~# wget https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.7/bin/apache-tomcat-10.1.7.tar.gz
		--2023-03-07 17:21:47--  https://dlcdn.apache.org/tomcat/tomcat-10/v10.1.7/bin/apache-tomcat-10.1.7.tar.gz
		Resolving dlcdn.apache.org (dlcdn.apache.org)... 2a04:4e42::644, 151.101.2.132
		Connecting to dlcdn.apache.org (dlcdn.apache.org)|2a04:4e42::644|:443... connected.
		HTTP request sent, awaiting response... 200 OK
		Length: 12143798 (12M) [application/x-gzip]
		Saving to: ‘apache-tomcat-10.1.7.tar.gz’

		apache-tomcat-10.1.7.tar.gz                        100%[===============================================================================================================>]  11.58M  9.93MB/s    in 1.2s    

		2023-03-07 17:21:48 (9.93 MB/s) - ‘apache-tomcat-10.1.7.tar.gz’ saved [12143798/12143798]

		root@nagaraju:~# ^C
		root@nagaraju:~# .
		
curl : it is command is used to transfer the fies.
  Ex : curl -V.
  
ping : command is used to test the connectivity between two networks.
     Ex : ping google.com.
     
uname : to display the user Name.
     Ex Uname.
     
Histiry : is used to show the history.
  Ex : history.
  
  ps ux : command that displays a list of all process running in the system, including their associate user and cpu/memory usage.
   Ex : pu us.root@nagaraju:~# ps ux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.1 169652 12696 ?        Ss   07:07   0:05 /sbin/init splash
root           2  0.0  0.0      0     0 ?        S    07:07   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        I<   07:07   0:00 [rcu_gp]

ps -ef|grep <pid> : used to for finding information about a specific process running in the linux system.
 Ex:    root@nagaraju:~# ps -ef|grep devops
	root       28669   22958  0 17:44 pts/0    00:00:00 grep --color=auto devops
	root@nagaraju:~# 

   
