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

$ ssh cs15lsp22zz@ieng6.ucsd.edu

This command line is an example. You would have to input your own username followed by @iend6.ucsd.edu. 

If this is your first time connecting, you should see this message. 

⤇ ssh cs15lsp22zz@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?

Type yes and enter. Then, it would ask for your password. Input the password, you used when obtaining your course specific account. Once you successfully typed your password, youw ould see this. 

<img width="698" alt="Screen Shot 2022-03-31 at 8 36 18 AM" src="https://user-images.githubusercontent.com/58501820/162518045-d02bf29f-dd16-4af5-9a42-72cd09d23ed4.png">

Now your terminal is connected to the computer in the CSE basement. Your computer will be the client and the computer in the basement is the server. 
---
### Part 3: Running Commands 



# Link To Report

[Lab Report 1 Google Doc](https://docs.google.com/document/d/1FjhcWWyNLU-B-I-_yEofumn0BLGZxYbWXScFVp-Wg_w/edit?usp=sharing)

---
### Screenshot from Lab 1 (Testing) 
<img width="698" alt="Screen Shot 2022-03-31 at 8 36 18 AM" src="https://user-images.githubusercontent.com/58501820/162236544-77eb0a25-b559-4fd8-8620-2d25dab3952b.png">


>*Remotly connecting using SSH*
