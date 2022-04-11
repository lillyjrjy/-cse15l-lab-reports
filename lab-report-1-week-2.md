# Week 2 Lab Report

## Installing VScode
---

1. [Download on VScode from website](https://code.visualstudio.com/)
2. Install on computer

<img width="461" alt="Screen Shot 2022-04-08 at 6 49 26 PM" src="https://user-images.githubusercontent.com/56412294/162551979-937047e8-6b48-4e6a-8667-a7e18cafa5f4.png">

## Remotely Connecting
---

1. enter on terminal, 
```
 ssh cs15lsp22zz@ieng6.ucsd.edu
```

2. Type yes to connect to the new server. Then enter password when prompted.

You should see something similar to the screenshpt below.

<img width="432" alt="Screen Shot 2022-04-08 at 7 30 02 PM" src="https://user-images.githubusercontent.com/56412294/162553450-4549d998-d9e1-47e4-a7e7-320f45ce2fc8.png">

## Trying Some Commands
---

commands that are useful form lab 1 writeup in class:

```
cd ~
cd
ls -lat
ls -a
ls <directory> where <directory> is /home/linux/ieng6/cs15lsp22/cs15lsp22abc, where the abc is one of the other group members’ username
cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/
cat /home/linux/ieng6/cs15lsp22/public/hello.txt
mv
mkdir
```
SImply type them out in terminal, example below:
<img width="540" alt="Screen Shot 2022-04-08 at 7 38 55 PM" src="https://user-images.githubusercontent.com/56412294/162553490-2f9f8412-d0fd-4004-9f9c-bcfc898aafdc.png">

## Moving Files with scp
---
1. Create a new file locally.
2. Using `scp FileName.java cs15lsp22alr@ieng6.ucsd.edu:~/` to transfer the file to ieng6.

<img width="542" alt="Screen Shot 2022-04-08 at 7 39 29 PM" src="https://user-images.githubusercontent.com/56412294/162553500-1218c230-40f9-439a-b59b-a2925e7583d7.png">


## Setting an SSH Key
---
1. On local computer, enter `$ ssh-keygen`
2. Create file to save the key `/Users/lillyyang/.ssh/id_rsa`
3. Log back to the server.
4. `$ mkdir .ssh`

5. On local computer, `scp /Users/lillyyang/.ssh/id_rsa.pub cs15lsp22alr@ieng6.ucsd.edu:~/.ssh/authorized_keys`


<img width="662" alt="Screen Shot 2022-04-08 at 7 40 13 PM" src="https://user-images.githubusercontent.com/56412294/162553513-e819b6e3-3610-4a2e-9ce6-76dfacd35b39.png">


## Optimizing Remote Running
---
1. enter `ssh cs15lsp22alr@ieng6.ucsd.edu "javac filename.java; java filename" `

Can copy file to server with one line of command.
<img width="667" alt="Screen Shot 2022-04-08 at 7 40 35 PM" src="https://user-images.githubusercontent.com/56412294/162553520-a788f93d-01f5-4741-add4-3e078e35b938.png">
