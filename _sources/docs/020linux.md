# Linux commands

## Ubuntu
### Installation
Update the OS
```
$ sudo apt-get update

$ sudo apt-get upgrade
```
Remove unnecessary files after an OS upgrade.
```
$ sudo apt-get autoremove
```
Install an app
```
$ sudo apt-get app_name
```
Check if program is installed
```
$ apt list --installed program_name
```
Remove program
```
$ sudo apt-get remove --auto-remove program_name
```

### File System
Check size of a directory
```
$ du -sh /path/to/folder
```
Check volumes in system
```
$ df -h
```
List a directory
```
$ ls
```
List with details, or show all hidden files
```
$ ls -lh file/foldername (will be able to see size in human readable way)

$ ls -l file/foldername

$ ls -la file/foldername
```
Copy file
```
$ cp /path/to/file1 /path/to/file2

$ cp -r /path/to/folder /path/to/folder

```
Remove a file.
```
$ rm filename
```
Create a file
```
# touch filename
```
Remove a folder.
```
$ rm -r foldername
$ rm -rf foldername #delete all folders in folders
```
Change permission
```
$ chmod g=rw filename
```
```
u=owner
g=group users
o=other users
a=all users

r=read
w=write
-=no permission
```
Add directory
```
$ sudo mkdir
```
Copy files from local machine to a remote machine
```
$ scp C:\local\machine\file\path username@chaosbox.com:/your/path/on/remote/machine
```


### Shellscript
Execute a shellscript
```
$ sudo sh shellscript_name
```

### Internet
Download a file from website with curl
```
$ curl -L https://github.com/chenkianwee/masa3db/archive/0.02.zip > masa3db-0.02.zip
```

### Read and Write Text
Read a text file
```
cat filename.txt
```
Create a text file
```
cat > filename.txt
```

### System
Check running service
```
$ systemctl status process_name
```
Stop running service
```
$ systemctl stop process_name
```
Start running service
```
$ systemctl start process_name
```
Check distribution
```
$ cat /etc/os-release
```

### Network
Get ip
```
hostname -i

hostname
```
