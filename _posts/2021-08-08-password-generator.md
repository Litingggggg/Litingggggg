---
layout: post
subtitle: with my first flowchart
categories: [Python, Flowchart]
header:
    image: header.jpg
    align:
    text: light
---

```python
import random

#设置string
digits = "0123456789"
capital_letter = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
lower_case = "abcdefghijklmnopqrstuvwxyz"
symbol = "!@#$%^&*"

print(" ")
print("Welcome to Password Generator. This is a simple programme ")
print("which help you generate your password automatically. ~~~~~")
print("The password could include digitals, capital letters, small")
print("letters and symbols. You can fully custom it by yourself.")
print("Enjoy :)")
print(" ")

# accept user input then cast(convert) to integer type and assign to variable password_length
password_length=int(input("How long of the password do you want to generate? \nPlease type a number: ")) 

# accept 
is_capital=input("Do you want to involve capital letters in your password? Y/N\n").strip().lower() 
is_lower=input("Do you want to involve lowercases in your password? Y/N\n").strip().lower()
is_symbol=input("Do you want to involve symbols in your password? Y/N\n").strip().lower()


final_password=""
option_str=digits

if is_capital == "y":
    # option_str=option_str+capital_letter
    option_str+=capital_letter

if is_lower == "y":
    option_str=option_str+lower_case

if is_symbol == "y":
    option_str=option_str+symbol


for i in range(password_length):
    random_index=random.randrange(0,len(option_str))
    final_password=final_password+option_str[random_index]

print("\nCongradulations! Your password has been generated successfully. \n%s" %(final_password))
print(" ")
#布尔boolean

```
{% include image.html img="flowchart_transparent_bg_with_shadow.png" alt="Flowchart" caption="Flowchart" %}



<iframe width="1280" height="720" src="https://www.youtube.com/embed/y8tF0yRl8-w" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>