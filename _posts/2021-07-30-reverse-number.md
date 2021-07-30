---
layout: post
subtitle: Python Algorithm
categories: [Python,CS101]
header:
    image: https://source.unsplash.com/4nulm-JUYFo.jpg
    align:
    text: light
---

Tings started with that I need to finish my first TimeCodeRunner exersice. I was lost when I opened the second question.

#### Question
*Given a 2 digit number write a program which:

retrieve the "tens" digit,
retrieve the "units" digit,
print the number in reverse order.*

## Code Below：

```python
n=input("Please input a number you wanna reversed: ") 
num=int(n)
rev=0  #define a variable rev and assign value to 0
while(num>0):
    rev=(rev*10)+(num%10)
    num=num//10
 
print("The number you input is %s, the reversed number is %s." %(n,rev))

```