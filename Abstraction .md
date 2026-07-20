# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math

# Abstract Class
class Shape(ABC):

    @abstractmethod
    def calculate_area(self):
        pass

# Rectangle Class
class Rectangle(Shape):
    def __init__(self):
        self.length = 10
        self.breadth = 5

    def calculate_area(self):
        print("Area of Rectangle =", self.length * self.breadth)

# Circle Class
class Circle(Shape):
    def __init__(self):
        self.radius = 7

    def calculate_area(self):
        print("Area of Circle =", round(math.pi * self.radius * self.radius, 2))

# Main Program
r = Rectangle()
c = Circle()

r.calculate_area()
c.calculate_area()
```
## Output
<img width="668" height="173" alt="image" src="https://github.com/user-attachments/assets/9da66a4b-fd4a-4b6c-a7fc-840b48dcd0e0" />

## Result
Thus, the abstract class Shape with the abstract method calculate_area() was successfully implemented, and the subclasses Rectangle and Circle correctly calculated and displayed their respective areas.
