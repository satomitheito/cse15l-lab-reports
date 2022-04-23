# Debugging 
## Satomi Ito
## A16157881



## Debug 1

When conducting 

`javac MarkdownParse.java`

and 

`java MarkdownParse test-file.md`

This is the error out put we are getting. 


<img width="546" alt="Screen Shot 2022-04-23 at 4 22 11 PM" src="https://user-images.githubusercontent.com/58501820/164949454-00956812-0ccf-4f38-ab23-5114b49d1579.png">

As you can see, it throws an OutOfMemoryError exception. This happened because the orginal code has a loop that was searching the test file, which caused an infinite loop. To solve this, we added an if statement to break the loop if the next line does not contain an `[`. 


<img width="711" alt="Screen Shot 2022-04-23 at 4 34 54 PM" src="https://user-images.githubusercontent.com/58501820/164949517-b45305e1-6d97-4eb6-b15d-2215e72feb6c.png">


<img width="484" alt="Screen Shot 2022-04-23 at 4 23 36 PM" src="https://user-images.githubusercontent.com/58501820/164949565-2e11f708-e9e2-4193-a7b1-6c77c3d2f389.png">




---

## Debug 2

---

## Debug 3
