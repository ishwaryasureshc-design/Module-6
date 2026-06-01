<img width="1213" height="637" alt="image" src="https://github.com/user-attachments/assets/17fbf589-da5d-4332-877e-7881e847881b" /># 🐍 Python OOP: Abstract Class & Method Example

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

class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

class Rectangle(Shape):
    def __init__(self, length=1, breadth=1):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
    def __init__(self, radius=1):
        self.radius = radius

    def calculate_area(self):
        return 3.14159 * self.radius * self.radius

rect = Rectangle(5, 3)
circle = Circle(4)

print("Rectangle Area:", rect.calculate_area())
print("Circle Area:", circle.calculate_area())
```

## Output

<img width="1213" height="637" alt="Screenshot 2026-06-01 140559" src="https://github.com/user-attachments/assets/1a4f2501-4f2a-4489-9bfd-66861c7e221e" />

## Result
The program defines an abstract class Shape and implements two subclasses, Rectangle and Circle, each providing its own calculate_area() method. It then calculates and displays the areas of a rectangle and a circle.
