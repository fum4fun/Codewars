# CodeWars Python Solutions

---

## Predict your age!


My grandfather always predicted how old people would get, and right before he passed away he revealed his secret!

In honor of my grandfather's memory we will write a function using his formula!

    -Take a list of ages when each of your great-grandparent died.
    -Multiply each number by itself.
    -Add them all together.
    -Take the square root of the result.
    -Divide by two.

Example

predict_age(65, 60, 75, 55, 60, 63, 64, 45) == 86

Note: the result should be rounded down to the nearest integer.

---

### Given Code

```python
def predict_age(age_1, age_2, age_3, age_4, age_5, age_6, age_7, age_8):
    # your code
```

---

### Solution

```python
import math
def predict_age(*ages):
    return math.floor(math.sqrt(sum(i * i for i in ages))/2)
```


---


[See on CodeWars.com](https://www.codewars.com/kata/5aff237c578a14752d0035ae/train/python)
