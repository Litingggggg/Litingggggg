---
layout: post
subtitle: Python Algorithm
categories: [Python]
header:
    image: https://source.unsplash.com/4nulm-JUYFo.jpg
    align:
    text: light
---

# Reversed Numbers

```python
n=input("Please input a number you wanna reversed: ") 
num=int(n)
rev=0  #define a variable rev and assign value to 0
while(num>0):
    rev=(rev*10)+(num%10)
    num=num//10
 
print("The number you input is %s, the reversed number is %s." %(n,rev))

```