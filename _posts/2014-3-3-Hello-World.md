---
layout: post
title: Python Practise-1
published: true
---
## This is my first post on python practise-1
### Lets start...

### 1.Fill in the blanks of this code to print out the numbers 1 through 7.
```python
   number = 1
while number <=7:
 print(number, end=" ")
 number+=1
```

#### Answer: 1 2 3 4 5 6 7

### 2.The show_letters function should print out each letter of a word on a separate line. Fill in the blanks to make that happen.
 ```python  	
        def show_letters(word):
 for letters in word:
 print(letters)
show_letters("Hello")
```
#### Answer: 
#### H
#### e
#### l
#### l
#### o

#### 3.Complete the function digits(n) that returns how many digits the number has. For example: 25 has 2 digits and 144 has 3 digits. Tip: you can figure out the digits of a number by dividing it by 10 once per digit until there are no digits left
```python      
      def digits(n):
 count = 0
 if n == 0:
 return 1
 while (int(n/10) != 0):
 count += 1
 n = int(n/10)
 return count+1
print(digits(25))
print(digits(144))
print(digits(1000))
print(digits(0))
```

##### Answer:2 3 4 1

#### 4.This function prints out a multiplication table (where each number is the result of multiplying the first number of its row by the number at the top of its column). Fill in the blanks so that calling multiplication_table(1,3) will print out:
1 2 3 
2 4 6
3 6 9
```python
    	def multiplication_table(start, stop):
 for x in range(start,stop+1):
 for y in range(start,stop+1):
 print(str(x*y), end=" ")
 print()
multiplication_table(1, 3)
```
##### Answer: Answer is given in question above

#### 5.The following code raises an error when executed. What's the reason for the error?
```python
    	def decade_counter():
 while year < 50:
 year += 10
 return year
```
##### Answer:Failure to initialize variables

#### 6.What is the value of x at the end of the following code?
```python  
 for x in range(1, 10, 3):
 print(x)
```
##### Answer:7

#### 7.What is the value of y at the end of the following code?
```python   	
for x in range(10):
 for y in range(x):
 print(y)
```
##### Answer:8
 
#### 8.How does this function need to be called to print yes, no, and maybe as possible options?
```python
def votes(params):
 for vote in params:
 print("Possible option:" + vote)
```
##### Answer: votes(['yes', 'no', 'maybe'])
