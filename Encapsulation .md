# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth
        print("Length:", self.__length)
        print("Breadth:", self.__breadth)

rect = Rectangle(10, 5)
```
## Output
<img width="1364" height="542" alt="Screenshot 2026-06-01 141009" src="https://github.com/user-attachments/assets/63fd653e-7929-4f23-b4c2-a87e594bbdff" />

## Result
The program defines a class Rectangle with two private attributes __length and __breadth. The constructor initializes these attributes and displays their values. When an object of the class is created, the constructor is automatically executed
