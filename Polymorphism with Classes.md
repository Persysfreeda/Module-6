# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
# Class Beans
class Beans:
    def type(self):
        print("Vegetable")

    def color(self):
        print("Green")

# Class Mango
class Mango:
    def type(self):
        print("Fruit")

    def color(self):
        print("Yellow")

# Generic Function
def func(obj):
    obj.type()
    obj.color()

# Main Program
obj1 = Beans()
obj2 = Mango()

func(obj1)
func(obj2)
```
## Output
<img width="681" height="187" alt="image" src="https://github.com/user-attachments/assets/2f2a56b9-fd89-4b7b-8c6b-d5b830726926" />

## Result
Thus, the Python program demonstrating polymorphism using the Beans and Mango classes with a generic function was successfully implemented.
