
# File Commamds

    • ls : The command is used  for in listing contents inside a directory.

  

    • cat : The Cat commamd is frequently used command to display the data of the file 
        Cat Filename. 
        Cat file2 enter.

  

    • more:  The more command is used to view the text files in the same command
     	 create some files 1,2,3,4,5,6 more file{1..5}.

    
    • tail :  The tail command is used to display the last 10 lines or 10 files .  tail file1

         .

    • tail -f : tail -f command can be used to monitor the growth of a file being written by another 
            process .
           tail -f file1

   
    • locate : The locate command finds files in Linux using
    • cd :  cd command is used to change the current working directory.
	cd .. - Change to the parent directory of the current working directory.
      cd ~ - Change to the home directory of the current user.
      cd / - Change to the root directory of the file system.


    •  mkdir : Create directory. 
                  Mkdir python.



    • touch : create emty files. 
             Touch file{1..5}.

    • move : The move is used to move one or more files or directories from one place to another.

            
    • rm : rm command is used to delete the file Ex : rm -r file name.

    • rmdir : command is used to remove a directory. It is a simple and straightforward command that removes the specified empty directory.
	rmdir directory.



    • Vi-Esc : The command moves the cursor from any position on that line. Press Esc to return to command mode after you type the desired text.
 Vi filename. 



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





grep : grep command filters the content of a file which makes our search easy . 
            grep keyword filename grep calss 2 is [keyword] file2 is [filename].


Grep -i : grep -i command is used to perform a case-insensitive search.
             grep -i "example" filename .  grep -i “hi” file2.
  
du : Du is is disk usage the du command is used to estimate file space usage.
	[du filename] .

       


df : disk file  usage This will display the disk space usage for the file system  
       that contains the specified directory. 
      df  -h /path/to/directory.

       

Diff : This command is used to find the difference between the file to file and 
         directories to directories.  
         diff file1 file2.




wc -l : This command in Linux is used to count the number of lines in a file.
          wc -l file2.

          


Tar : This command is used to create, manipulate, and extract files from tar archives. 
           Create file tar -cf mytar_tar filename.
           Extrat tar -xvf archive.tar 
           add  tar -rvf achive.tar file1 file2
           compress tar – czvf achive.tar.gz file1 file2.

Zip : A zip archive is a collection of files that are compressed and combined into a single
         file for easy distribution or backup.
        create a new zip : zip archive.zip file1 file2 devops.
        extract the contents of a zip : unzip archive.zip.
        add files to an existing zip : zip -r archive.zip file3 devops2.
        compress a zip : zip -9 archive.zip file1 file2 devops 1

unzip :  used to extract files from a compressed zip archive.
             unzip archive.zip

ln : command is used to create links to files or directories.

User Management

useradd : command to create a new user account.
                 sudo useradd raju 
		sudo useradd mk
		sudo useradd hk.
                 
passwd : This command is used to delete the existing user.
  		sudo passwd mk
		sudo passwd hk

userdel :  to verify deletion is complete or not
		Sudo userdel mk
		sudo userdel hk

           

