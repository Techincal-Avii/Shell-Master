Userstand the Linux folders:- 
erabh@Abhi:/mnt/c/Users/erabh/Shell-Master$ 
Admintrative User, @, Hostname, :(seperator
), /(this the path or present working directory, everything will be stored in this path)
~(Tilt is the home directory)
-----------------------------------------------------------------
ls ( list command) - ltr (All directories)
all System libraries and utilites are stored in these root folders.
To switch to the root user - we have sudo command (superdo)  [sudo su -]
Binary - these are the excutable files.
-----------------------------------------------------------------
Thses are the root folder : -
-rwxr-xr-x   1 root root 2781568 Dec 12 01:58 init
drwxr-xr-x   2 root root    4096 Apr 20 08:46 boot
lrwxrwxrwx   1 root root       8 Apr 20 08:46 sbin -> usr/sbin
lrwxrwxrwx   1 root root       7 Apr 20 08:46 lib -> usr/lib
lrwxrwxrwx   1 root root       9 Apr 20 08:46 lib64 -> usr/lib64
lrwxrwxrwx   1 root root       7 Apr 20 08:46 bin -> usr/bin
drwxr-xr-x   2 root root    4096 Apr 20 18:05 srv
drwxr-xr-x   2 root root    4096 Apr 20 18:05 opt
drwxr-xr-x   2 root root    4096 Apr 20 18:05 media
drwxr-xr-x  12 root root    4096 Apr 20 18:05 usr
drwx------   2 root root   16384 May 26 06:01 lost+found
drwxr-xr-x   5 root root    4096 May 26 06:01 mnt
drwxr-xr-x  13 root root    4096 May 26 06:02 var
drwxr-xr-x   2 root root    4096 May 26 06:02 snap
dr-xr-xr-x 257 root root       0 May 26 06:13 proc
drwxr-xr-x  15 root root    3920 May 26 06:13 dev
dr-xr-xr-x  13 root root       0 May 26 06:22 sys
drwx------   3 root root    4096 May 26 06:27 root
drwxr-xr-x  23 root root     640 May 26 06:46 run
drwxr-xr-x   4 root root    4096 May 26 06:46 home
drwxr-xr-x  89 root root    4096 May 26 06:46 etc
drwxrwxrwt   7 root root     140 May 26 06:55 tmp
-----------------------------------------------------------------
Folder 1 - sbin -> usr/sbin  (These are system binaries or system commands binaries that helps us to mangethe system )
Folder 2 - lib -> usr/lib - these are libraries
Folder 3 - boot - when the linux start or restart 
Folder - 4 - bin - bin stands for user binaries these are non administrative
Folder - 5 - usr - contain s administartivre and non administrative users
Folder - 6- srv - this is server folder where we can store configuration of the servers.
Folder -6- opt - id we have to install thired party tool or custom tool we have to goto to /opt and will create directory. thois is central loaction for all thired party tools.
Folder - 7- mnt - this is mount folder to add temprary storage to mount new volume 
Folder - 8- var - to store log files (the log of the webserver are stores on /var/log) or some libraries thired party
Folder - 9 - home - to craete or add new user 
Folder -10 - data -  to store any type of data 
Folder -11- proc - virtual file system 
Folder- 12- tmp - thse are temprary files or used to store temprary files
Folder - 13-  root-  thses is the home dirsctory
Folder - 14- run - thses store the run time data within in run folder
Folder - 15- etc- in linux all system configuration files of linux are stored in etc folder. (m ost imp files of the linux system)
[root@Abhi:/# echo $PATH
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin] when we see command not found so this is the path where ls commands works.

