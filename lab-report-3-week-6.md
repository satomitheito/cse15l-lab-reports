## Satomi Ito
## A16157881

### Streamlining ssh Configuration

<img width="475" alt="Screen Shot 2022-05-08 at 1 11 18 PM" src="https://user-images.githubusercontent.com/58501820/167314164-f0f02377-4004-45a7-bc20-0a71fed04ab7.png">

<img width="564" alt="Screen Shot 2022-04-28 at 9 45 15 AM" src="https://user-images.githubusercontent.com/58501820/167313323-1ebf134b-2dca-4236-a1ac-09592c8c7168.png">

<img width="688" alt="Screen Shot 2022-05-08 at 12 15 00 PM" src="https://user-images.githubusercontent.com/58501820/167313328-59d1db99-91a1-41d9-8bb2-1a65065a73af.png">

<img width="599" alt="Screen Shot 2022-05-08 at 12 46 25 PM" src="https://user-images.githubusercontent.com/58501820/167313334-3450f066-b687-4a44-ac6e-2aa01c356153.png">


<img width="652" alt="Screen Shot 2022-05-08 at 12 46 10 PM" src="https://user-images.githubusercontent.com/58501820/167313341-c282d5c6-457f-4809-aa0b-48bac95b6d52.png">

---

### Setup Github Access from ieng6

<img width="778" alt="Screen Shot 2022-05-08 at 1 14 07 PM" src="https://user-images.githubusercontent.com/58501820/167316158-149ecdca-5f4b-4df2-8caf-de6c7c0d3826.png">

<img width="430" alt="Screen Shot 2022-05-08 at 1 06 28 PM" src="https://user-images.githubusercontent.com/58501820/167316163-22727390-58af-4d6b-80cf-acfda5255805.png">

<img width="478" alt="Screen Shot 2022-05-08 at 2 38 31 PM" src="https://user-images.githubusercontent.com/58501820/167316883-58de3564-2e53-478f-a872-2622b84de498.png">

Midway I realised my token expired so I had to regenerate a new token and authenticate it. 

<img width="528" alt="Screen Shot 2022-05-08 at 2 39 06 PM" src="https://user-images.githubusercontent.com/58501820/167316887-ca525983-d4c3-49e9-86a5-6612a2fde4ad.png">

[here](https://github.com/satomitheito/markdown-parser)

---

### Copy whole directories with `scp -r`


`scp -r . cs15lsp22amn@ieng6.ucsd.edu:~/markdown-parse; ssh ieng6 "cd markdown-parse; /software/CSE/oracle-java-17/jdk-17.0.1/bin/javac -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar MarkdownParseTest.java; /software/CSE/oracle-java-17/jdk-17.0.1/bin/java -cp .:lib/junit-4.13.2.jar:lib/hamcrest-core-1.3.jar org.junit.runner.JUnitCore MarkdownParseTest"`

