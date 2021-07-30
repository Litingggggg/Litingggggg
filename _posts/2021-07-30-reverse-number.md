---
layout: post
subtitle: Python Algorithm
categories: [Python,CS101]
header:
    image: https://source.unsplash.com/4nulm-JUYFo.jpg
    align:
    text: light
---

Things started with that I need to finish my first TimeCodeRunner exercise. I was lost when I opened the second question.

*Given a two-digit number, write a program that retrieves the "tens" digit, retrieves the "units" digit, and prints the number in reverse order.*

### How to reverse a number?

I went to check all the lectures mentioned in the project description. However, there is no explanation. 

I struggled. 

By rechecking the question, *You need to use the modulus (%) and floor division (//) operators in your calculations.* I used the two methods to write the answer.

```python
import math

number = xx

tens_digit=number//10
units_digit=number%10

print("The reversed number is: %s%s"%(units_digit,tens_digit))
```

It works well. So it looks like to reverse a number, we only need to find those "tens" digits by divided the number given by ten and find those "units" digit by the remainders of the number provided divided by 10. 

However, it only works with two-digit numbers. Once the number is a three-digit number, the whole system would dead.

### How to reverse a Multiple-digit Number

For doing this, I learned to draw a flowchart at first.

#### Draw a flowchart
By checking the website ASQ, we can get more idea about the flowchart:
[https://asq.org/quality-resources/flowchart]

The flowchart is a picture of the separate steps of a process in sequential order. it is made up by mulytiply shapes, use these and those arrows together can draw a fine flowchart.

The flowchart is a picture of the separate steps of a process in sequential order. It is making of multiple shapes, use these and those arrows together can draw an exemplary flowchart.

* Oval-shaps: start and endpoints 
* Parallelograms: estimate 
* Rectangles: progress 
* Rhombus: judge, estimate 
* Arrows: the direction the process goes

In this case here, we want a progress can reverse all numbers no matter how many digits they are. 




#### Code：

```python
n=input("Please input a number you wanna reversed: ") 
num=int(n)
rev=0  #define a variable rev and assign value to 0
while(num>0):
    rev=(rev*10)+(num%10)
    num=num//10
 
print("The number you input is %s, the reversed number is %s." %(n,rev))

```