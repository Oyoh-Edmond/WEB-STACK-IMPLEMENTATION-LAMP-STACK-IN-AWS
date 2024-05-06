# Self Study

## Chown & Chmod

Use the `chown` command to change file owner and group information.

We run the `chmod` command command to change file access permissions such as read (r), write (w), and execute (x) permission.

## Understanding file permissions for chmod and chown command
We use file permissions to control access to files. Sysadmins can enforce a security policy based upon file permissions. All files have three types:

**Owner** – Person or process who created the file.

**Group** – All users have a primary group, and they own the file, which is useful for sharing files or giving access.

**Others** – Users who are not the owner, nor a member of the group. Also, know as world permission.

`User permissions -> Group permissions -> Other permissions`



`r` - Reading access/view file	- Users can read file. In other words, they can run the ls command to list contents of the folder/directory.

`w`	- Writing access/update/remove file	- Users can update, write and delete a file from the directory.

`x`	- Execution access. Run a file/script as command - Users can execute/run file as command and they have r permission too.

`-`	- No access. When you want to remove r, w, and x permission	- All access is taken away or removed.

### CHOWN command

```bash
touch demo.txt     ##create a file

ls -l demo.txt  ## list permissions for demo.txt

Sample output:
-rw-r--r-- 1 Edmond 197121 0 May  6 01:14 demo.
```
_from the above: `Edmond` is the owner of this file_

```bash
sudo cut -d: -f1 /etc/passwd  ##list users 

sudo chown root demo.txt ##change ownership to root 

Sample output:
-rw-r--r-- 1 root 0 May  6 01:38 demo.txt
```

### CHMOD command

#### We use the following letters for user:

`u` for user

`g` for group

`o` for others

`a` for all

#### We can set or remove (user access rights) file permission using the following letters:

`+` for adding

`-` for removing

`=` set exact permission

#### File permission letter is as follows:

`r` for read-only

`w` for write-only

`x` for execute-only



```bash
touch script.sh

ls -l script.sh  #-rw-r--r-- 1 eddy eddy 245 May  6 01:45 script.sh

./script.sh ## execute script - Permission denied

chmod +x script.sh 
 
./script.sh
```