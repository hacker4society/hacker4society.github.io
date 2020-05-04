---
published: true
layout: post
description: pyton programming
date: 2020-05-03T00.00.0000Z
tags:
  - programming
---
##### 1.What's the value of this Python expression: "big" > "small" ?
#### Answer:False

##### 2.What is the elif keyword used for?
#### Answer:To handle more than two comparison cases.

##### 3.Students in a class receive their grades as Pass/Fail. Scores of 60 or more (out of 100) mean that the grade is "Pass". For lower scores, the grade is "Fail". In addition, scores above 95 (not included) are graded as "Top Score". Fill in this function so that it returns the proper grade.
```Python3
def exam_grade(score):
	if score>95:
		grade = "Top Score"
	elif score>=60:
		grade = "Pass"
	else:
		grade = "Fail"
	return grade

print(exam_grade(65)) # Should be Pass
print(exam_grade(55)) # Should be Fail
print(exam_grade(60)) # Should be Pass
print(exam_grade(95)) # Should be Pass
print(exam_grade(100)) # Should be Top Score
print(exam_grade(0)) # Should be Fail
```
#### Answer:Pass
#### Fail
#### Pass
#### Pass
#### Top Score
#### Fail

<!--more-->

##### 4.What's the value of this Python expression: 11 % 5?
#### Answer:1

##### 5.The longest_word function is used to compare 3 words. It should return the word with the most number of characters (and the first in the list when they have the same length). Fill in the blank to make this happen.
```Python3
def longest_word(word1, word2, word3):
	if len(word1) >= len(word2) and len(word1) >= len(word3):
		word = word1
	elif len(word2)>=len(word3):
		word = word2
	else:
		word = word3
	return(word)

print(longest_word("chair", "couch", "table"))
print(longest_word("bed", "bath", "beyond"))
print(longest_word("laptop", "notebook", "desktop"))
```
#### Answer:chair
#### beyond
#### notebook

##### 6.What’s the output of this code?
```Python3
def sum(x, y):
	return(x+y)
print(sum(sum(1,2), sum(3,4)))
```
#### Answer:10

##### 7.What's the value of this Python expression?
`((10 >= 5*2) and (10 <= 5*2))`

#### Answer:True

##### 8.The fractional_part function divides the numerator by the denominator, and returns just the fractional part (a number between 0 and 1). Complete the body of the function so that it returns the right number. Note: Since division by 0 produces an error, if the denominator is 0, the function should return 0 instead of attempting the division.
```Python3
def fractional_part(numerator, denominator):
     return float((numerator % denominator)) / denominator  if denominator != 0 
       else 0
print(fractional_part(5, 5)) # Should be 0
print(fractional_part(5, 4)) # Should be 0.25
print(fractional_part(5, 3)) # Should be 0.66...
print(fractional_part(5, 2)) # Should be 0.5
print(fractional_part(5, 0)) # Should be 0
print(fractional_part(0, 5)) # Should be 0
```
#### Answer: 0 , 0.25 , 0.66... , 0.5 , 0 , 0 and answer shown in comment also.
