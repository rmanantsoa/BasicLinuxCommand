# BasicLinuxCommand [Unix/Linux Command Reference]
##  File Commands
- ls :   Directory listing
- ls -al  : Formatted listing with hidden files
- ls -lt : Sorting the Formatted listing by time modification
- cd dir : Change directory to dir
- cd Change : to home directory
- pwd : Show current working directory
- mkdir dir : Creating a directory dir
- cat > file : Places the standard input into the file
- more file : Output the contents of the file
- head file :  Output the first 10 lines of the file
- tail file :  Output the last 10 lines of the file
- tail -f file :  Output the contents of file as it grows,starting with last 10 lines
- touch file :  Create or update file
- rm file :  Deleting the file
- rm -r dir :  Deleting the directory
- rm -f file :  Force to remove the file
- rm -rf dir :  Force to remove the directory dir
- cp file1 file2 :  Copy the contents of file1 to file2
- cp -r dir1 dir2 :  Copy dir1 to dir2;create dir2 if not present
- mv file1 file2 :  Rename or move file1 to file2,if file2 is an existingdirectory
- ln -s file link :  Create symbolic link link to file

## Process management
- ps : To display the currently working processes
- top : Display all running process
- kill pid : Kill the process with given pid
- killall proc : Kill all the process named proc
-  pkill pattern : Will kill all processes matching the pattern
- bg : List stopped or background jobs,resume a stopped job in the background
- fg : Brings the most recent job to foreground
- fg n : Brings job n to the foreground

## File permission
- chmod (octal file) : Change the permission of file to octal,which can be found separately for user,group,world by adding, 4-read(r), 2-write(w), 1-execute(x)

## Searching
- grep pattern file : Search for pattern in file
- grep -r pattern dir : Search recursively for pattern in dir
- command | grep  pattern : Search pattern in the output of a command
- locate file : Find all instances of file
- find .-name filename  Searches in the current directory (represented by a period) and below it, for files and directories with names starting with filename
- pgrep pattern : Searches for all the named processes , that matches with the pattern and, by default, returns their ID

## System Info
- date : Show the current date and time
- cal : Show this month's calender
- uptime :Show current uptime
- w : Display who is on line
- whoami : Who you are logged in as Unix/Linux Command Reference 
- finger user : Display information about user
- uname -a : Show kernel information
- cat /proc/cpuinfo : show Cpu information
- cat proc/meminfo : show Memory information
- man command : Show the manual for command
- df : Show the disk usage
- du : Show directory space usage
- free : Show memory and swap usage
- whereis app : Show possible locations of app
- which app : Show which applications will be run by default

## Compression
- tar cf file.tar file : Create tar named file.tar containing file
- tar xf file.tar : Extract the files from file.tar
- tar czf file.tar.gz files : Create a tar with Gzip compression
- tar xzf file.tar.gz : Extract a tar using Gzip
- tar cjf file.tar.bz2 : Create tar with Bzip2 compression
- tar xjf file.tar.bz2 : Extract a tar using Bzip2
- gzip file : Compresses file and renames it to file.gz
- gzip -d file.gz : Decompresses file.gz back to file

## Network
- ping host : Ping host and output results
- whois domain : Get whois information for domains
- dig domain : Get DNS information for domain
- dig -x host : Reverse lookup host
- wget file : Download file
- wget -c file:  Continue a stopped download
- netstat : displays various network related information such as network connections, routing tables, interface statistics, masquerade connections, ... 
- nslookup : used to obtain information about Internet servers. As its name suggests, the utility finds name server information for domains by querying DNS

## Shortcuts
- ctrl+c : Halts the current command
- ctrl+z : Stops the current command, resume with fg in the foreground or bg in the background
- ctrl+d Logout the current session, similar to exit
- ctrl+w : Erases one word in the current line
- ctrl+u : Erases the whole line
- ctrl+r : Type to bring up a recent command
- !! :  Repeats the last command
- exit : Logout the current session




