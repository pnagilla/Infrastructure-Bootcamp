Linux Commands:


Display the current directory path.
[bob@centos-host tmp]$ pwd
/tmp

Check your location after changing directories.
[bob@centos-host bin]$ pwd
/lib/debug/bin



Use pwd after navigating to /etc.
[bob@centos-host etc]$ pwd
/etc

List all files in the current directory.
[bob@centos-host tmp]$ ls
linux                                                                    systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi

List files with detailed info (ls -l).
[bob@centos-host tmp]$ ls -l
total 16
drwxr-xr-x. 2 bob  bob  4096 Aug  2 04:51 linux
drwx------. 3 root root 4096 Aug  2 03:56 systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8
drwx------. 3 root root 4096 Aug  2 03:56 systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
drwx------. 3 root root 4096 Aug  2 03:56 systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi
[bob@centos-host tmp]$ 


List hidden files (ls -a).
[bob@centos-host tmp]$ ls -a
.   linux                                                                    systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
..  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi
[bob@centos-host tmp]$ 

List files sorted by modification time (ls -t).
[bob@centos-host tmp]$ ls -t
linux                                                                           systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8
systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
[bob@centos-host tmp]$ 

List files in a specific directory, e.g., /var/log.
[bob@centos-host log]$ ls -lart
total 240
drwxr-x---.  2 chrony chrony   4096 Jun 19  2024 chrony
drwxr-xr-x.  2 root   root     4096 Jul 15  2024 qemu-ga
drwxr-x---.  2 sssd   sssd     4096 Jul 22  2024 sssd
-rw-------.  1 root   root        0 Jul 24  2024 tallylog
lrwxrwxrwx.  1 root   root       39 Jul 24  2024 README -> ../../usr/share/doc/systemd/README.logs
drwx------.  2 root   root     4096 Jul 24  2024 private
-rw-rw----.  1 root   utmp        0 Jul 24  2024 btmp
drwx------.  3 root   root     4096 Jul 24  2024 samba
-rw-------.  1 root   root        0 Jul 24  2024 maillog
-rw-------.  1 root   root        0 Jul 24  2024 spooler
drwxr-xr-x.  2 root   root     4096 Jul 24  2024 anaconda
drwx------.  2 root   root     4096 Aug  2 03:56 audit
drwxr-xr-x. 19 root   root     4096 Aug  2 03:56 ..
-rw-rw-r--.  1 root   utmp     2304 Aug  2 03:56 wtmp
drwxr-xr-x.  9 root   root     4096 Aug  2 03:56 .
-rw-r--r--.  1 root   root     1550 Aug  2 04:33 dnf.rpm.log
-rw-r--r--.  1 root   root      600 Aug  2 04:33 hawkey.log
-rw-r--r--.  1 root   root     9842 Aug  2 04:33 dnf.librepo.log
-rw-r--r--.  1 root   root    19748 Aug  2 04:33 dnf.log
-rw-rw-r--.  1 root   utmp   292876 Aug  2 04:46 lastlog
-rw-------.  1 root   root     9637 Aug  2 04:46 secure
-rw-------.  1 root   root     1330 Aug  2 04:51 cron
-rw-------.  1 root   root   137053 Aug  2 04:54 messages

List all files, including hidden ones.
[bob@centos-host log]$ ls -lart
total 240
drwxr-x---.  2 chrony chrony   4096 Jun 19  2024 chrony
drwxr-xr-x.  2 root   root     4096 Jul 15  2024 qemu-ga
drwxr-x---.  2 sssd   sssd     4096 Jul 22  2024 sssd
-rw-------.  1 root   root        0 Jul 24  2024 tallylog
lrwxrwxrwx.  1 root   root       39 Jul 24  2024 README -> ../../usr/share/doc/systemd/README.logs
drwx------.  2 root   root     4096 Jul 24  2024 private
-rw-rw----.  1 root   utmp        0 Jul 24  2024 btmp
drwx------.  3 root   root     4096 Jul 24  2024 samba
-rw-------.  1 root   root        0 Jul 24  2024 maillog
-rw-------.  1 root   root        0 Jul 24  2024 spooler
drwxr-xr-x.  2 root   root     4096 Jul 24  2024 anaconda
drwx------.  2 root   root     4096 Aug  2 03:56 audit
drwxr-xr-x. 19 root   root     4096 Aug  2 03:56 ..
-rw-rw-r--.  1 root   utmp     2304 Aug  2 03:56 wtmp
drwxr-xr-x.  9 root   root     4096 Aug  2 03:56 .
-rw-r--r--.  1 root   root     1550 Aug  2 04:33 dnf.rpm.log
-rw-r--r--.  1 root   root      600 Aug  2 04:33 hawkey.log
-rw-r--r--.  1 root   root     9842 Aug  2 04:33 dnf.librepo.log
-rw-r--r--.  1 root   root    19748 Aug  2 04:33 dnf.log
-rw-rw-r--.  1 root   utmp   292876 Aug  2 04:46 lastlog
-rw-------.  1 root   root     9637 Aug  2 04:46 secure
-rw-------.  1 root   root     1330 Aug  2 04:51 cron
-rw-------.  1 root   root   137053 Aug  2 04:54 messages

Create a directory named project.
[bob@centos-host tmp]$ ls
linux    systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8      systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi
project  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
[bob@centos-host tmp]$ 

Remove the directory project.
[bob@centos-host tmp]$ rm -r project
[bob@centos-host tmp]$ ls
linux                                                                    systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-dbus-broker.service-LTotDz
systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-chronyd.service-XJFMq8  systemd-private-8a2d0ec1624e4a81b537ad1d2967fc85-systemd-logind.service-JU8Iyi
[bob@centos-host tmp]$ 

Create an empty file called file1.txt.
[bob@centos-host linux]$ touch pranaya.txt
[bob@centos-host linux]$ 

Copy file1.txt to file2.txt.
[bob@centos-host linux]$ cp pranaya.txt pranaya2.txt

Rename file1.txt to renamed.txt.
[bob@centos-host linux]$ mv pranaya.txt lin.txt
[bob@centos-host linux]$ ls
lin.txt  pranaya2.txt

Delete renamed.txt.
[bob@centos-host linux]$ rm lin.txt 
[bob@centos-host linux]$ ls
pranaya2.txt


Find all .log files in /var/log.
Com: find /var/log -type f -name "*.log"
Display the contents of file.txt. 
[bob@centos-host linux]$ cat pranaya2.txt 
wgjdvnm

Show the first 10 lines of file.txt.
 head -10 filename
Show the last 10 lines of file.txt.
 tail -10 filename

Display the size of file.txt.  
Ls -l or ls -lh
Display disk usage of the current directory.
Du -h
Change directory to the root directory /.
Cd /.
List files in /etc.
Ls /etc
List files in /home.
Ls /home
List files in /bin.
Ls /bin
Change directory to /tmp.
Cd /tmp
Create a symbolic link to file.txt named link_to_file.
Sym link : type of the file which acts a pointer to another file/directory
Ln -s filename symlinkfilename(new)
[bob@centos-host linux]$ ln -s pranaya2.txt lin.txt
[bob@centos-host linux]$ ls
lin.txt  pranaya2.txt

Remove the symbolic link.
Rm symlink
[bob@centos-host linux]$ rm lin.txt 
[bob@centos-host linux]$ ls
pranaya2.txt

Display hidden files in the current directory.
Ls -a

Change directory to the previous directory.
Cd ..

Create a directory with spaces in its name: My Projects.
Mkdir "My Projects"

Change into My Projects.
Cd 'My Projects'

Clear the terminal screen.
clear

Display the current user's username.
who

Display the current date and time.
date

Display the current user's home directory path.
 echo ~username
 
List files sorted by name in reverse order.
Ls -l | sort -r

Change directory to the root of the filesystem.
Cd /.

List all mounted filesystems.
Mount -l

Find the size of a directory and its contents.
Du -sh directoryname

Create a file named test.txt with some text.
Echo "hai" > filename

Append text to test.txt.
Echo "content" >> filename

Remove a file named oldfile.txt.
 rm oldfile.txt
 
Create a directory named my_folder.
 mkdir my_folder
 
Create nested directories: parent/child.
 mkdir -p dir1/dir2
 
Create multiple directories at once: dir1 dir2 dir3.
 mkdir dir1 dir2 dir3
 
Create a directory with spaces in its name: "My Folder".
  mkdir "MY Folder"
  
Create a directory with specific permissions: mkdir -m 755 new_dir.
 mkdir -m 755 dirname
 
Exit the terminal.
  exit
