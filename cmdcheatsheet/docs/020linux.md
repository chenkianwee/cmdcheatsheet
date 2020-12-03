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
### File System
List a directory
```
$ ls
```
List with details, or show all hidden files
```
$ ls -l file/foldername

$ ls -la file/foldername
```
Remove a file.
```
$ rm filename
```
Remove a folder.
```
$ rm -r foldername
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
