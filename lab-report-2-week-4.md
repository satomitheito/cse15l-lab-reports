# Debugging 
## Satomi Ito
## A16157881

This is the link to the original markdown parse [here](https://github.com/nidhidhamnani/markdown-parser/blob/main/MarkdownParse.java)


This is the link to the test file [here](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-file.md)

## Debug 1

When conducting 

`javac MarkdownParse.java`

and 

`java MarkdownParse test-file.md`

This is the error out put we are getting. 


<img width="546" alt="Screen Shot 2022-04-23 at 4 22 11 PM" src="https://user-images.githubusercontent.com/58501820/164949454-00956812-0ccf-4f38-ab23-5114b49d1579.png">

There is an OutOfMemoryError exception thrown. This happened because the orginal code has a loop that was searching the test file, which caused an infinite loop. To solve this, we added an if statement to break the loop if the next line does not contain an `[`. 


<img width="711" alt="Screen Shot 2022-04-23 at 4 34 54 PM" src="https://user-images.githubusercontent.com/58501820/164949517-b45305e1-6d97-4eb6-b15d-2215e72feb6c.png">


<img width="484" alt="Screen Shot 2022-04-23 at 4 23 36 PM" src="https://user-images.githubusercontent.com/58501820/164949565-2e11f708-e9e2-4193-a7b1-6c77c3d2f389.png">


---

## Debug 2

There is another test file that we are going to test. [Here](https://github.com/satomitheito/markdown-parser/blob/main/test-file2.md)

When conducting 

`javac MarkdownParse.java`

and 

`java MarkdownParse test-file2.md`

This is the error out put we are getting. 


<img width="703" alt="Screen Shot 2022-04-23 at 5 08 18 PM" src="https://user-images.githubusercontent.com/58501820/164950244-bcc51a6a-e64b-4bfd-86fa-89b07aa4d60c.png">

There is aa StringIndexOutOfBoundsException thrown due to the code unable to find the `[` in the test file. Therefore, we have to create an if statement in a while loop that considered the lack of `[` and causes the loop the break and returning an empty arraylist.

<img width="707" alt="Screen Shot 2022-04-23 at 5 06 56 PM" src="https://user-images.githubusercontent.com/58501820/164950252-3c725f7a-3a40-4080-bb75-577b5e1aebad.png">


<img width="491" alt="Screen Shot 2022-04-23 at 5 07 56 PM" src="https://user-images.githubusercontent.com/58501820/164950253-172ed617-64b6-41bf-8aa5-4d2bdb8ee6c6.png">


---

## Debug 3

When conducting 

`javac MarkdownParse.java`


