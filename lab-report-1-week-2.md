# **Remote Access**
## Satomi Ito 
## A16157881

### Part 1: Visual Studio Code
Make sure you have Visual Studio Code downloaded. If not, download from [here](https://code.visualstudio.com/). Open the application.

<img width="1143" alt="Screen Shot 2022-03-31 at 8 21 27 AM" src="https://user-images.githubusercontent.com/58501820/162517801-454e333c-8e55-4428-9d12-68ab0ae9084d.png">

---

### Part 2: Remotely Connecting 
To get your course specific account, click on this link:

https://sdacs.ucsd.edu/~icc/index.php

You should be able to get your username, which would look something like this:

cs15lsp22zz

Then, in Visual Studio Code, open the terminal (Ctrl + `, or Terminal → New Terminal menu) Input command:


> $ ssh cs15lsp22zz@ieng6.ucsd.edu


This command line is an example. You would have to input your own username followed by @iend6.ucsd.edu. 

If this is your first time connecting, you should see this message. 


> ⤇ ssh cs15lsp22zz@ieng6.ucsd.edu

> The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.

> RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.

> Are you sure you want to continue connecting (yes/no/[fingerprint])?


Type yes and enter. Then, it would ask for your password. Input the password, you used when obtaining your course specific account. Once you successfully typed your password, you would see this. if ran successful, your terminal will be connected to the computer in the CSE basement. Your computer will be the client and the computer in the basement is the server.

<img width="698" alt="Screen Shot 2022-03-31 at 8 36 18 AM" src="https://user-images.githubusercontent.com/58501820/162518045-d02bf29f-dd16-4af5-9a42-72cd09d23ed4.png">
 
---
### Part 3: Running Commands 
These are some useful commands. 

> cd ~

> cd

> ls -lat

> ls -a

> ls <directory> where <directory> is /home/linux/ieng6/cs15lsp22/cs15lsp22abc, where the abc is one of the other group members’ username

> cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/

>cat /home/linux/ieng6/cs15lsp22/public/hello.txt

<img width="727" alt="Screen Shot 2022-03-31 at 8 48 16 AM" src="https://user-images.githubusercontent.com/58501820/162518803-d129acaa-590c-4d3e-b3ee-270738437cf6.png">


<img width="542" alt="Screen Shot 2022-03-31 at 9 09 03 AM" src="https://user-images.githubusercontent.com/58501820/162518828-8aee2a02-a2f0-4a63-95c7-90d98b91748c.png">

To log out of the remote server in your terminal, you can use:

Ctrl-D

Run the command exit 

---

### Part 4: Moving Files over SSH with scp

Log out of your remote server in your terminal by following the instruction given above. Then, Create a file on your computer called WhereAmI.java and put the following code into it:


class WhereAmI {

  public static void main(String[] args) {
  
    System.out.println(System.getProperty("os.name"));
    
    System.out.println(System.getProperty("user.name"));
    
    System.out.println(System.getProperty("user.home"));
    
    System.out.println(System.getProperty("user.dir"));
    
  }
  
}
 
 
On the terminal, cd into the area where the file is. Then, run this command. 

> scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/

Again , cs15lsp22zz should be different for everyone based on what they get on the course specific account. After inputting your password. Log into ieng6 with ssh again. Your terminal should look like this. 

For refresher, this is the ssh code:

> $ ssh cs15lsp22zz@ieng6.ucsd.edu

If ran successfully, you should see this output. 

<img width="1004" alt="Screen Shot 2022-03-31 at 9 13 21 AM" src="https://user-images.githubusercontent.com/58501820/162520774-bd1bd5dc-e6bb-46b2-bc07-fa512219a59d.png">

To run the file on the ieng6 computer, run javac and then java. Below should be the output. 


<img width="370" alt="Screen Shot 2022-03-31 at 9 14 55 AM" src="https://user-images.githubusercontent.com/58501820/162520958-f99ace4d-9155-4da1-80bc-2b397e910114.png">

---

### Part 5: SSH Keys

This step will let you run ssh and scp without inputting your password everytime. First, log out of the remote server on your terminal. Then on terminal, input this following command.

> $ ssh-keygen

If ran successfully, this would be the output. 

<img width="504" alt="Screen Shot 2022-03-31 at 9 22 04 AM" src="https://user-images.githubusercontent.com/58501820/162547244-27e678d7-a927-44e5-9536-e375aa46186f.png">

This created two new files on your system; the private key (in a file id_rsa) and the public key (in a file id_rsa.pub), stored in the .ssh directory on your computer. Follow the following commands. 

> $ ssh cs15lsp22zz@ieng6.ucsd.edu

You will need to input the password one last time. 

> <Enter Password>

> now on server

> $ mkdir .ssh

> logout

> back on client

> $ scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys

> You use your username and the path you saw in the command above

> Once you do this, you should be able to ssh or scp from this client to the server without entering your password.

<img width="789" alt="Screen Shot 2022-03-31 at 9 35 35 AM" src="https://user-images.githubusercontent.com/58501820/162547397-358ef0ad-13aa-47f5-9156-b86b2be0c438.png">

---



# Link To Report

[Lab Report 1 Google Doc](https://docs.google.com/document/d/1FjhcWWyNLU-B-I-_yEofumn0BLGZxYbWXScFVp-Wg_w/edit?usp=sharing)

---
### Screenshot from Lab 1 (Testing) 
<img width="698" alt="Screen Shot 2022-03-31 at 8 36 18 AM" src="https://user-images.githubusercontent.com/58501820/162236544-77eb0a25-b559-4fd8-8620-2d25dab3952b.png">


>*Remotly connecting using SSH*
