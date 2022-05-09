## Satomi Ito
## A16157881

### Streamlining ssh Configuration

I used text edit to edit this config file. 
<img width="475" alt="Screen Shot 2022-05-08 at 1 11 18 PM" src="https://user-images.githubusercontent.com/58501820/167314164-f0f02377-4004-45a7-bc20-0a71fed04ab7.png">

<img width="564" alt="Screen Shot 2022-04-28 at 9 45 15 AM" src="https://user-images.githubusercontent.com/58501820/167313323-1ebf134b-2dca-4236-a1ac-09592c8c7168.png">



`ssh ieng6`

<img width="688" alt="Screen Shot 2022-05-08 at 12 15 00 PM" src="https://user-images.githubusercontent.com/58501820/167313328-59d1db99-91a1-41d9-8bb2-1a65065a73af.png">



I made a java file and copied a file to the account.

<img width="599" alt="Screen Shot 2022-05-08 at 12 46 25 PM" src="https://user-images.githubusercontent.com/58501820/167313334-3450f066-b687-4a44-ac6e-2aa01c356153.png">


<img width="652" alt="Screen Shot 2022-05-08 at 12 46 10 PM" src="https://user-images.githubusercontent.com/58501820/167313341-c282d5c6-457f-4809-aa0b-48bac95b6d52.png">

---

### Setup Github Access from ieng6

Public Key 

<img width="778" alt="Screen Shot 2022-05-08 at 1 14 07 PM" src="https://user-images.githubusercontent.com/58501820/167316158-149ecdca-5f4b-4df2-8caf-de6c7c0d3826.png">


Private Key (Represented by id_rsa.pub)


<img width="430" alt="Screen Shot 2022-05-08 at 1 06 28 PM" src="https://user-images.githubusercontent.com/58501820/167316163-22727390-58af-4d6b-80cf-acfda5255805.png">


I created a java file and add, commit, and pushed it to the markdown-parser.

<img width="478" alt="Screen Shot 2022-05-08 at 2 38 31 PM" src="https://user-images.githubusercontent.com/58501820/167316883-58de3564-2e53-478f-a872-2622b84de498.png">

Midway I realised my token expired so I had to regenerate a new token and authenticate it. 

<img width="528" alt="Screen Shot 2022-05-08 at 2 39 06 PM" src="https://user-images.githubusercontent.com/58501820/167316887-ca525983-d4c3-49e9-86a5-6612a2fde4ad.png">

Result:

[here](https://github.com/satomitheito/markdown-parser)

---

### Copy whole directories with `scp -r`

Copied the whole markdown-parse directory to the ieng6 account.

The command `scp -r . cs15lsp22amn@ieng6.ucsd.edu:~/markdown-parse` allows us to copy whole directories into the ieng6 account.

<img width="683" alt="Screen Shot 2022-05-08 at 2 42 05 PM" src="https://user-images.githubusercontent.com/58501820/167326282-42600bfa-8db2-468d-9552-679eb9271967.png">


Logged into the ieng6 account after doing this and compiling and running the tests for the repository.


<img width="698" alt="Screen Shot 2022-05-08 at 2 43 30 PM" src="https://user-images.githubusercontent.com/58501820/167326305-39546ba2-d179-4936-aebf-95832359ebae.png">


Combined scp, ;, and ssh to copy the whole directory and run the tests in one line

`scp -r . cs15lsp22amn@ieng6.ucsd.edu:~/markdown-parse; ssh ieng6 "cd markdown-parse; /software/CSE/oracle-java-17/jdk-17.0.1/bin/javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; /software/CSE/oracle-java-17/jdk-17.0.1/bin/java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`

<img width="690" alt="Screen Shot 2022-05-08 at 6 35 36 PM" src="https://user-images.githubusercontent.com/58501820/167326226-bda3885a-b683-4a10-a93c-fdd308c47255.png">


<img width="696" alt="Screen Shot 2022-05-08 at 6 35 44 PM" src="https://user-images.githubusercontent.com/58501820/167326232-a6dd86b7-6d15-4086-8168-47fae29cbacb.png">



