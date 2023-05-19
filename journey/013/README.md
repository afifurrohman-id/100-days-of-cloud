![image](https://user-images.githubusercontent.com/118882411/211846448-06c566be-1da5-4bee-a374-0cd0c2276e79.png)

# Meet 2 | User & Groups managements, Permission (Chown - Chmod - Chgrp)

## Introduction

Continue linux fundamentals, now learn about about File Access Managements, User & Groups and basic command to change owner or groups files includes change permissions files . The journey will be like this:

- User & Groups Management
- Permissions (Chmod - Chown - Chgrp)

## Cloud Research

### User

User just like a account, in linux you can create more than one users
<br> <b>NOTE: All commands in this session need privileges from administrator (root)</b>
to create users in linux u can use two options: <br>

1. use <code>useradd</code> command <br>
2. use <code>adduser</code> command <br>
   what is the difference between the two commands? <br> <code>useradd</code> create user without password, home directory, and more specific about information user
   <br> For example:<br>
   ![image](https://user-images.githubusercontent.com/118882411/211849788-6939ad80-768e-4fd6-8297-f269039341cd.png)
   <br><br>while the <code>adduser</code> command is used to create an administrative user, this user has the password, home directory as well as other information<br>
   For example:<br>
   ![image](https://user-images.githubusercontent.com/118882411/211850363-1e417d9d-424b-4f93-a5b8-971318ab1be2.png)

To login user using <code>su</code> command<br>
![image](https://user-images.githubusercontent.com/118882411/211851483-7fbadd20-e649-43a4-ae0a-45bf6b5796cc.png)

Use <code>userdel -m</code> to delete user with home directory
![image](https://user-images.githubusercontent.com/118882411/211856083-8703bc7f-2b6d-436e-85a5-5df5cb7653bd.png)

### Group

To create groups in linux using <code>groupadd</code> command, just like creating a users
<br>And use <code>groupadd</code> command to add user to a groups
![image](https://user-images.githubusercontent.com/118882411/211854730-6b43b573-3c7d-40f5-91d3-57fa3367562c.png)

<br>Use <code>delgroup</code> to delete group<br>
![image](https://user-images.githubusercontent.com/118882411/211856361-9c59f268-5666-4337-a671-3192559c6521.png)

### Permissions

![image](https://user-images.githubusercontent.com/118882411/211840733-f68a8d0d-f25a-4ef5-a439-37d89992b822.png)

• So what does the red marker in the image above mean? we will discuss it one by one.
the <code>-rw-rw-rwx 1 afif afif 32 jan 11 21:55 hello.sh</code>

<code>rwx</code> : r = read permission, w = write, x = execute

First <code>-</code> is Files type, if first <code>d</code> is a directory, or <code>l</code> is a linking
<br><code>rw-</code> Is a permission for owner file
<br><code>rw-</code> Permission for groups
<br><code>rw-</code> Permission for other
<br><code>afif</code> Owner file(user)
<br><code>afif</code> Groups file
<br><code>32 jan 11 21:55</code> File creation time
<br><code>hello.sh</code> File name

use <code>chmod</code> command to change permission file
<br> here <code>chmod</code> have 2 options to change permission file:

> Use Numeric (r/read=4, w/write=2, x/execute=1) use like this <code>chmod 751</code> ><br> ![image](https://user-images.githubusercontent.com/118882411/211861577-d2c67c26-d2c6-4eb7-aa2a-772dea117c19.png) ><br> Use Alphabetic. You can use + - or = , just like this<br> >![image](https://user-images.githubusercontent.com/118882411/211861975-c0f568b5-ff5d-43e4-b002-707b41b8f1ef.png)

Use <code>chown</code> to change owner<br>
![image](https://user-images.githubusercontent.com/118882411/211863016-720dba08-fa79-46e9-b0ae-2f3f1aa4bc2d.png)
<br>Add <code>:</code> to change group<br>
![image](https://user-images.githubusercontent.com/118882411/211863460-8cd2569e-41b7-44f1-b276-06b3fd2e1e5f.png)

Also you can use <code>chgrp</code> to change group<br>
![image](https://user-images.githubusercontent.com/118882411/211864952-59d80990-2e78-453a-8ca0-d17883657c5c.png)

## Next Steps

- EC2 Instance Connect & EC2 Instances Purchasing Options

