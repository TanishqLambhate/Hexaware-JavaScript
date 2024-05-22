## defer
- If the defer attribute is set, it specifies that the script is downloaded in parallel to parsing the page, and executed after the page has finished parsing.
```js
<script defer>
```
```js
class Car {
        constructor(name, engine, wheels, doors) {
          this.name = name;
          this.engine = engine;
          this.wheels = wheels;
          this.doors = doors;
        }
 
        horn() {
          return `${this.name} says Vroom Vroom!!!`;
        }
      }
 
      ferrari = new Car("Ferrari", "v8", 4, 2); // object (instance)
      alto = new Car("Alto", "v4", 4, 4); // object
      console.log(ferrari);
      console.log(alto);
      console.log(typeof Car, typeof ferrari, typeof alto);

class Item { constructor(name, quantity) { this.name = name; this.quantity = quantity; this.constructor.count++; } static count = 0; static getCount() { return Item.count; } } let pen = new Item('Pen', 5); let notebook = new Item('notebook', 10); console.log(Item.getCount()); // 2
```
```python
# Inheritance
class Animal:
    def __init__(self, name):
        self._name = name
 
    # methods / attributes
    def speak(self):
        return "Some sound"
 
 
class Dog(Animal):
    def __init__(self, name, speed):
        super().__init__(name)  # Base class constructor
        self.__speed = speed
 
    def run(self):
        return "🐶 wags tail!!"
 
    # Polymorphism:  Method overriding
    def speak(self):
        return "Woof!! 🐕"
 
    def speed_bonus(self):
        return f"{self._name} is running at {self.__speed * 2}Km/hr"
 
 
toby = Animal("toby")
print(toby.speak())
# print(toby.run())
 
maxy = Dog("maxy", 20)
# print(maxy._name)
print(maxy.run())
print(maxy.speak())
# print(maxy.__speed)
print(maxy.speed_bonus())
```