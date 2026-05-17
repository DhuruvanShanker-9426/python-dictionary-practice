# 🐍 Python Dictionary Practice

## 📌 Project Overview

This repository contains beginner-friendly Python dictionary practice exercises.

The main goal of this practice is to understand how dictionaries work in Python, including key-value pairs, accessing values, updating data, deleting items, looping through dictionaries, counting word frequency, finding maximum values, and working with nested dictionaries.

---

## 🎯 Objectives

- Understand Python dictionary syntax
- Create dictionaries using key-value pairs
- Access values using keys
- Add new key-value pairs
- Update existing dictionary values
- Delete dictionary items
- Loop through keys, values, and key-value pairs
- Count word frequency using dictionaries
- Find the key with the highest value
- Work with nested dictionaries

---

## 🧠 Concepts Practiced

### 1. Creating a Dictionary

Created a dictionary to store student details such as name, age, course, and city.

```python
student = {
    "name": "Dhuru",
    "age": 21,
    "course": "Data Science",
    "city": "Coimbatore"
}
```

---

### 2. Accessing Dictionary Values

Accessed dictionary values using the dictionary key and dictionary methods.

```python
print(student["name"])
print(student["course"])
print(student["city"])
```

Example output:

```text
Dhuru
Data Science
Coimbatore
```

The `.values()` method can also be used to get all values from the dictionary.

```python
student.values()
```

---

### 3. Adding New Key-Value Pairs

Added a new key called `skills` with a list of values.

```python
student["skills"] = ["Python", "SQL", "Power BI"]
```

---

### 4. Updating Dictionary Values

Updated the course value from `Data Science` to `AI and ML`.

```python
student["course"] = "AI and ML"
```

---

### 5. Deleting Dictionary Items

Deleted the `city` key from the dictionary.

```python
del student["city"]
```

---

### 6. Looping Through Dictionary Keys

Used a loop to print all dictionary keys.

```python
for key in student:
    print(key)
```

Example output:

```text
name
age
course
skills
```

---

### 7. Looping Through Dictionary Values

Used the `.values()` method to print all values.

```python
for value in student.values():
    print(value)
```

---

### 8. Looping Through Key-Value Pairs

Used the `.items()` method to print both keys and values.

```python
for key, value in student.items():
    print(key, ":", value)
```

Example output:

```text
name : Dhuru
age : 21
course : AI and ML
skills : ['Python', 'SQL', 'Power BI']
```

---

## 🔢 Word Frequency Counting

Used a dictionary to count how many times each word appears in a list.

```python
words = ["python", "sql", "python", "powerbi", "sql", "python"]

word_freq = {}

for word in words:
    if word in word_freq:
        word_freq[word] += 1
    else:
        word_freq[word] = 1

print(word_freq)
```

Output:

```python
{'python': 3, 'sql': 2, 'powerbi': 1}
```

---

## 🏆 Finding the Highest Mark

Used the `max()` function with `key=marks.get` to find the subject with the highest mark.

```python
marks = {
    "Maths": 90,
    "Python": 95,
    "SQL": 85,
    "Power BI": 88
}

top_subject = max(marks, key=marks.get)

print(top_subject, ":", marks[top_subject])
```

Output:

```text
Python : 95
```

Explanation:

```python
max(marks, key=marks.get)
```

This finds the key whose value is maximum.

In this example, `Python` has the highest mark, so it returns `Python`.

---

## 🧩 Nested Dictionary

Created a dictionary inside another dictionary to store multiple student details.

```python
students = {
    "student1": {
        "name": "Dhuru",
        "age": 21,
        "course": "Data Science"
    },
    "student2": {
        "name": "Arun",
        "age": 22,
        "course": "Python"
    }
}

print(students["student1"]["name"])
print(students["student2"]["name"])
```

Output:

```text
Dhuru
Arun
```

---

## 📚 Key Learnings

- A dictionary stores data in key-value format.
- Keys should be unique.
- Values can be strings, numbers, lists, or another dictionary.
- `.keys()` returns all keys.
- `.values()` returns all values.
- `.items()` returns key-value pairs.
- Dictionaries are useful for storing structured data.
- Dictionaries are helpful for counting repeated values.
- Nested dictionaries are useful for storing complex data like multiple student records.

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook

---

## 📁 File Included

```text
dict_practice.ipynb
```

---

## ✅ Conclusion

This practice helped me understand the basics of Python dictionaries and how they can be used for real-world data handling tasks such as storing student details, counting word frequency, finding maximum values, and working with nested data structures.