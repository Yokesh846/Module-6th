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
    def get_type(self):
        return "Vegetable"

    def get_color(self):
        return "Green"

# Class Mango
class Mango:
    def get_type(self):
        return "Fruit"

    def get_color(self):
        return "Yellow"

# Generic function using polymorphism
def display_info(obj):
    print("Type :", obj.get_type())
    print("Color:", obj.get_color())
    print()

# Create objects
bean = Beans()
mango = Mango()

# Call generic function
display_info(bean)
display_info(mango)
```

## Output
```
Type : Vegetable
Color: Green

Type : Fruit
Color: Yellow
```
## Result
The output has been verified successfully.
