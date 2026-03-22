# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
```
import re

def filter_without_e(words):

    pattern = re.compile(r'^[^eE]*$')
    
   
    return [word for word in words if pattern.match(word)]

words_list = ["apple", "sky", "dog", "tree", "milk", "sun"]
result = filter_without_e(words_list)

print("Original list:", words_list)
print("Filtered list (without 'e'):", result)
```

## Output
<img width="767" height="295" alt="image" src="https://github.com/user-attachments/assets/f41bc2a8-6ee0-440d-8f84-0c9803ed9ea8" />

## Result
thus the program is executed successfully.
