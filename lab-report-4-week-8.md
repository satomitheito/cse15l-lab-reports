# Snippet 
## Satomi Ito
## A16157881

Click [here](https://github.com/satomitheito/markdown-parser) for my markdown respository. 

Click [here](https://github.com/yuxinguo13/markdown-parser.git) for the one we reviewed in week 7

---

## Snippet 1

```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```


<img width="502" alt="Screen Shot 2022-05-22 at 4 45 46 PM" src="https://user-images.githubusercontent.com/58501820/169721232-465d2fca-23c8-4e4c-b232-d5c4097ccf5f.png">


<img width="686" alt="Screen Shot 2022-05-22 at 4 43 38 PM" src="https://user-images.githubusercontent.com/58501820/169721159-647bb3a2-2834-4b2b-b015-08e7a2808188.png">


### Implementation

<img width="503" alt="Screen Shot 2022-05-22 at 5 07 10 PM" src="https://user-images.githubusercontent.com/58501820/169722182-c07a4910-6f8b-4b1f-9cc3-aa91c02b3608.png">


<img width="604" alt="Screen Shot 2022-05-22 at 5 07 17 PM" src="https://user-images.githubusercontent.com/58501820/169722184-fd039c55-51a8-4903-aae9-e141c2b8f32c.png">

Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

I do not think that a small code change will make my program work. I would need to ad more conditions that considers the ` as some of them are in places outside of the bracket. 

---

## Snippet 2

```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```

<img width="512" alt="Screen Shot 2022-05-22 at 5 01 57 PM" src="https://user-images.githubusercontent.com/58501820/169721942-e7803a96-36db-405e-a8ac-d44dfdeb93ef.png">


<img width="688" alt="Screen Shot 2022-05-22 at 5 02 09 PM" src="https://user-images.githubusercontent.com/58501820/169721946-076aa455-917c-4121-955c-a8dfdc941e58.png">


### Implementation

<img width="508" alt="Screen Shot 2022-05-22 at 5 08 36 PM" src="https://user-images.githubusercontent.com/58501820/169722240-95ebcc0e-e4c5-4b07-b0dc-bf4af65faaf8.png">


<img width="524" alt="Screen Shot 2022-05-22 at 5 08 30 PM" src="https://user-images.githubusercontent.com/58501820/169722235-04e3fe86-2ad6-4f57-be98-12f864008f56.png">


Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

I think a small code change can make the program work. This is because unlike snippet 1, there is no ` that are outside the brackets and the only thing to consider is the (()). 

---

## Snippet 3

```[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```



<img width="695" alt="Screen Shot 2022-05-22 at 5 04 37 PM" src="https://user-images.githubusercontent.com/58501820/169722081-07ed94e4-34f3-48dd-929a-8cd8d467bc41.png">


<img width="857" alt="Screen Shot 2022-05-22 at 5 04 48 PM" src="https://user-images.githubusercontent.com/58501820/169722088-48d8d94a-d3b5-4d2a-a464-a933529354a6.png">


### Implementation 

<img width="697" alt="Screen Shot 2022-05-22 at 5 09 27 PM" src="https://user-images.githubusercontent.com/58501820/169722265-ea0f3627-44f8-4630-99f2-b8e5dc56148a.png">


<img width="581" alt="Screen Shot 2022-05-22 at 5 09 59 PM" src="https://user-images.githubusercontent.com/58501820/169722281-5fce494b-a0ad-4e0d-b8b5-df3d7bd13784.png">

Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

I think a small code change will be enough to make the program work as the only thing I would need to consider is a line break. 


