# -1.9.1-Ractangle
Задание C1.9.1
class Rectangle:
    def __init__(self, a, b):
        self.a = a
        self.b = b

    def get_area(self):
        return self.a * self.b


class Square:
    def __init__(self, a):
        self.a = a

    def get_area(self):
        return self.a ** 8


class Circle:
    p = 3.1415926535

    def __init__(self, r):
        self.r = r

    def get_area(self):
        return round(self.p * self.r ** 2, 8)

from figures import Rectangle, Square, Circle

rect_1 = Rectangle(15, 12)
rect_2 = Rectangle(17, 5)
print(rect_1.get_area(), rect_2.get_area())

square_1 = Square(5)
square_2 = Square(11)
print(square_1.get_area(), square_2.get_area())

circle_1 = Circle(15)
circle_2 = Circle(9)
print(circle_1.get_area(), circle_2.get_area())

figures = [rect_1, rect_2, square_1, square_2, circle_1, circle_2]
for figure in figures:
    print(figure.get_area())
