# python-code
PS:Print anagrams together in Python using List and Dictionary
s = ['cat', 'dog', 'tac', 'god', 'act']
d= {}
for i in s:
    k = ''.join(sorted(i))
    if k in d:
        d[k].append(i)
    else:
        d[k] = [i]
print(d)
print(list(d.values())) 

PS:Check if binary representations of two numbers are an anagram
num1=int(input('enter the first no.:'))
num2=int(input('enter the second no.:'))
if (''.join(sorted(bin(num1))))==(''.join(sorted(bin(num2)))):
    print('no.s are anagram')
else:
    print('no.s are not anagram')
    
PS:Python Counter to find the size of the largest subset of anagram words
 s='ant magenta magnate tan gnamate nat ant'
dict={}
count=0
for i in s.split():
    k=(''.join(sorted(i)))
    if k in dict:
        dict[k].append(i)
        
    else:
        dict[k]=[i]
print(dict)
print(len(max(dict.values())))

Write a Python function to find the Max of three numbers.
def max(x,y,z):
    if x>y and x>z:
        return x
    elif y>x and y>z:
        return y
    else: 
        return z
print(max(-1,6,4))

Write a Python function to sum all the numbers in a list.
l=[1,2,3,4,5,6,7]
def sum_num(l):
    sum=0
    for i in l:
        sum=sum+i
    print(sum)
sum_num(l)
l=[1,2,3,4,5,6,7]
from functools import reduce
fun=lambda x,y:x+y
reduce(fun,l)

Write a Python function to multiply all the numbers in a list.
l=[1,2,3,4,5,6,7]
from functools import reduce
fun=lambda x,y:x*y
reduce(fun,l)

Write a Python program to reverse a string.###While loop
s='pooja'
c=len(s)-1
rev_s=''
while c>=0:
    rev_s=rev_s+(s[c])
    c-=1 
print(rev_s)

.Write a Python function to find the Max of three numbers.
def max(x,y,z):
    if x>y and x>z:
        return x
    elif y>x and y>z:
        return y
    else: 
        return z
print(max(-1,6,4))

Write a Python function to sum all the numbers in a list.
l=[1,2,3,4,5,6,7]
from functools import reduce
fun=lambda x,y:x+y
reduce(fun,l)

#4.Write a Python program to reverse a string.###While loop
s='pooja'
c=len(s)-1
rev_s=''
while c>=0:
    rev_s=rev_s+(s[c])
    c-=1 
print(rev_s)

Write a Python function to calculate the factorial of a number (a non-negative integer).The function accepts the number as an argument.
num=int(input('enter the no.:'))
def fact(num):
    factorial=1
    if num<0:
        print('It is negative no.')
    else:
        while num>0:
            factorial=factorial*num
            num-=1
        print(factorial)
fact(num)

Write a Python program to find all words starting with 'a' or 'e' in a given string.
s='all peoples are enter in enthusiastic park'
print(' '.join([i for i in (s.split()) if i.startswith('a') or i.startswith('e')]))

Write a Python function to check whether a number falls in a given range.
def falls(num):
    if num in range(1,11):
        print('number falls in a given range.')
    else:print ("number not falls in a given range.")
falls(0)

Write a Python program to convert a date or yyyy-mm-dd format to dd-mm-yyyy
import datetime
input = '2021/05/25'
format = '%Y/%m/%d'
datetime = datetime.datetime.strptime(input, format)
print(datetime.date())

Write a Python program to replace whitespaces with an underscore and vice versa
str='Python Exercise_'
print((str.replace(' ','_')).replace('_',' '))
