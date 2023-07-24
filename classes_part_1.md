# Classes (part 1)

You can image a class as a blueprint for a house. The blueprint contains all the information about the house, but it is not a house itself. You can use the blueprint to build a house. The house is an instance of the blueprint. You can build as many houses as you want, but you always use the same blueprint. The blueprint is the class and the house is the instance of the class. It does not mean that all the houses are the same. You can build different houses from the same blueprint. You can change the color of the house, the number of rooms, the size of the windows, etc. The same is true for classes. You can create different instances of the same class and they can have different attributes and methods.

```python
class House():
    def __init__(self, color, number_of_rooms):
        self.color = color
        self.number_of_rooms = number_of_rooms

    def paint(self, new_color):
        self.color = new_color

    def add_room(self):
        self.number_of_rooms += 1

    def describe(self):
        print(f'This is a {self.color} house with {self.number_of_rooms} rooms.')
```

The class `House` has two attributes: `color` and `number_of_rooms`. The `__init__` method is called when you create a new instance of the class. It sets the initial values of the attributes. The `self` parameter is a reference to the instance of the class. It is used to access the attributes and methods of the instance. The `paint` method changes the color of the house. The `add_room` method adds a room to the house. The `describe` method prints a description of the house.

```python
house1 = House('red', 3)
house1.describe()

house2 = House('blue', 2)
house2.describe()

house1.paint('green')
house1.add_room()
house1.describe()
```

The output of the code above is:

```
This is a red house with 3 rooms.
This is a blue house with 2 rooms.
This is a green house with 4 rooms.
```

The `house1` and `house2` variables are instances of the `House` class. They have different values for the attributes `color` and `number_of_rooms`. The `describe` method prints the values of the attributes. The `paint` method changes the value of the `color` attribute. The `add_room` method increases the value of the `number_of_rooms` attribute by one.
