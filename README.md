# HACKER-RANK
#PRINT HELLO WORLD CODE:
if __name__ == '__main__':
    print("Hello, World!")

# PYTHON If-Else:

import math
import os
import random
import re
import sys


if __name__ == '__main__':
    n = int(input().strip())
    if n%2!=0:
        print("Weird")
    else:
        if n>=2 and n<=5:
            print("Not Weird")
        else:
            if n>=6 and n<=20:
                print("Weird")
            else:
                print("Not Weird")
    
# ARITHMATIC OPERATOR
if __name__ == '__main__':
    a = int(input())
    b = int(input())
    print(a+b)
    print(a-b)
    print(a*b)


# PYTHON DIVISION:

if __name__ == '__main__':
    a = int(input())
    b = int(input())
    print(a//b)
    print(a/b)

# LOOP:
if __name__ == '__main__':
    n = int(input())
    if n>=0:
        for i in range(n):
            print(i**2)

#Write a function:
def is_leap(year):
    leap = False
    if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
        leap = True
    return leap

year = int(input())
print(is_leap(year))

# Print FUNCTION:

if __name__ == '__main__':
    n = int(input())
    for i in range(1,n+1):
        print(i,end="")

# Find the Runner-up scored:

if __name__ == '__main__':
    n = int(input())
    arr = map(int, input().split())
    runner_up=sorted(list(set(arr)))[-2]
    print(runner_up)


# SWAPCASE CODE:

def swap_case(s):
    a=s.swapcase()
    return a

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)


# Finding the percentage

if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    avg=sum(student_marks[query_name])/(len(student_marks[query_name]))
    print("{:.2f}".format(avg))
