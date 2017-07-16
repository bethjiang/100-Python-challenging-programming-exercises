# 100-Python-challenging-programming-exercises
1. convert a list to dic
a = [1,2,3]
b = ['a','b','c']

D = dict(zip(b,a))
print(D)

2. Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5,
between 2000 and 3200 (both included).
The numbers obtained should be printed in a comma-separated sequence on a single line.

a = []
for i in range(2000,3201):
    if i % 7 == 0 and i % 5 != 0:
        a.append(i)
print(a)

3. Question:
Write a program which can compute the factorial of a given numbers.
The results should be printed in a comma-separated sequence on a single line.
Suppose the following input is supplied to the program:
8
Then, the output should be:
40320

def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(8))

4.Question:
With a given integral number n, write a program to generate a dictionary that contains (i, i*i) 
such that is an integral number between 1 and n (both included). 
and then the program should print the dictionary.
Suppose the following input is supplied to the program:
8
Then, the output should be:
{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}

def dict(n):
    d = {i:i*i for i in range(1,n+1)}
    return d

print(dict(8))

5.Question:
Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple 
which contains every number.
Suppose the following input is supplied to the program:
34,67,55,33,12,98
Then, the output should be:
['34', '67', '55', '33', '12', '98']
('34', '67', '55', '33', '12', '98')

def values(name):
    d = name.split(",")
    print(list(d))
    print(tuple(d))

values("34,67,55,33,12,98")

6.Question:
Define a class which has at least two methods:
getString: to get a string from console input
printString: to print the string in upper case.
Also please include simple test function 
to test the class methods.
class Hel:
    def __init__(self,value):
        self.data = value

    def getString(self):
        return self.data

    def printString(self):
        return self.data.upper()

    def test(self):
        pass

d = input("what do you want to input?")
x = hel(d)
print(x.printString())
print(x.getString())

7.Write a program that calculates and prints the value according to the given formula:
Q = Square root of [(2 * C * D)/H]
Following are the fixed values of C and H:
C is 50. H is 30.
D is the variable whose values should be input to your program in a comma-separated sequence.
Example
Let us assume the following comma separated input sequence is given to the program:
100,150,180
The output of the program should be:
18,22,24

