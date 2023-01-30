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
