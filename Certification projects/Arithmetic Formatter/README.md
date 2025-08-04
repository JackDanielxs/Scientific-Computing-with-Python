# Arithmetic Formatter 🧮

A Python function that formats and arranges arithmetic problems (addition and subtraction) vertically and side-by-side, just like students do in primary school.
---



## 📌 Features

- Supports up to **five** arithmetic problems at once.
- Handles **addition** and **subtraction** operations.
- Optional flag to **display answers**.
- Formats numbers neatly and consistently.
---

## 🧪 Example

### Function Call

```python

print(arithmetic\_arranger(\["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]))

```

### Output

```
   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
```

### With Answers

```python
print(arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"], True))
```

```
   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
  730      3799      88      172
```

---



## ⚠️ Input Validation

The function will return an error message in the following cases:

- More than 5 problems:  
&nbsp; `Error: Too many problems.`

- Unsupported operators (only `+` and `-` allowed):  
&nbsp; `Error: Operator must be '+' or '-'.`

- Non-digit characters in numbers:  
&nbsp; `Error: Numbers must only contain digits.`

- Numbers longer than four digits:  
&nbsp; `Error: Numbers cannot be more than four digits.`

---

## 📂 Usage

```python

from arithmetic_formatter import arithmetic_arranger
problems = ["32 + 698", "3801 - 2", "45 + 43", "123 + 49"]
print(arithmetic_arranger(problems, show_answers=True))

```

---
