---
layout: post
title: python practise 3
description: pyton programming
date: 2020-05-02T00:00:00.000Z
feature_image: null
tags:
  - programming
published: true
---

##### 1.The format_address function separates out parts of the address string into new strings:house_number and street_name, and returns: "house number X on street named Y". The format of the input string is: numeric house number, followed by the street name which may contain numbers, but never by themselves, and could be several words long. For example, "123 Main Street", "1001 1st Ave", or "55 North Center Drive". Fill in the gaps to complete this function.
```python
def format_address(address_string):
 # Declare variables
 house_number =''
 street_name =''
 # Separate the address string into parts
 spi = address_string.split()
 # Traverse through the address parts
 for ele in spi:
 # Determine if the address part is the
 # house number or part of the street name
 if ele.isdigit():
 house_number = ele
 else:
 street_name += ele
 street_name += ' '
 # Does anything else need to be done
 # before returning the result?

 # Return the formatted string
 return "house number {} on street named {}".format(house_number, street_nam
print(format_address("123 Main Street"))
# Should print: "house number 123 on street named Main Street"
print(format_address("1001 1st Ave"))
# Should print: "house number 1001 on street named 1st Ave"
print(format_address("55 North Center Drive"))
# Should print "house number 55 on street named North Center Drive"
def highlight_word(sentence, word):
 return(sentence.replace(word,word.upper()))
print(highlight_word("Have a nice day", "nice"))
print(highlight_word("Shhh, don't be so loud!", "loud"))
print(highlight_word("Automating with Python is fun", "fun"))
```
##### Answer:
- house number 123 on street named Main Street
- house number 1001 on street named 1st Ave 
- house number 55 on street named North Center Drive


##### 2.The highlight_word function changes the given word in a sentence to its upper-case version. For example, highlight_word("Have a nice day", "nice") returns "Have a NICE day". Can you write this function in just one line?
```python
def highlight_word(sentence, word):
 return(sentence.replace(word,word.upper()))
print(highlight_word("Have a nice day", "nice"))
print(highlight_word("Shhh, don't be so loud!", "loud"))
print(highlight_word("Automating with Python is fun", "fun"))
```
##### Answer:
- Have a NICE day
- Shhh, don't be so LOUD!
- Automating with Python is FUN

##### 3.A professor with two assistants, Jamie and Drew, wants an attendance list of the students, in the order that they arrived in the classroom. Drew was the first one to note which students arrived, and then Jamie took over. After the class, they each entered their lists into the computer and emailed them to the professor, who needs to combine them into one, in the order of each student's arrival. Jamie emailed a follow-up, saying that her list is in reverse order. Complete the steps to combine them into one list as follows: the contents of Drew's list, followed by Jamie's list in reverse order, to get an accurate list of the students as they arrived.
```python
def combine_lists(list1, list2):
 # Generate a new list containing the elements of list2
 # Followed by the elements of list1 in reverse order
 new_list = list2
 for i in reversed(range(len(list1))):
 new_list.append(list1[i])
 return new_list

Jamies_list = ["Alice", "Cindy", "Bobby", "Jan", "Peter"]
Drews_list = ["Mike", "Carol", "Greg", "Marcia"]
print(combine_lists(Jamies_list, Drews_list))
```
##### Answer:`['Mike', 'Carol', 'Greg', 'Marcia', 'Peter', 'Jan', 'Bobby', 'Cindy', 'Alice']`

##### 4.What do the following commands return when animal = "Hippopotamus"?
```python
>>> print(animal[3:6])
>>> print(animal[-5])
>>> print(animal[10:])
```
#### Answer:`pop, t, us`

##### 5.What do the following commands return? 
```python
host_addresses = {"router": "192.168.1.1", "localhost": "127.0.0.1", "google"
 "8.8.8.8"}
host_addresses.keys()
```
##### Answer: `['router', 'localhost', 'google']`
