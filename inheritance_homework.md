```.py
class Airplane:
    def __init__(self, brand, model, type, size:str, speed):
        self.brand = brand
        self.model = model
        self.type = type
        self.fuel_tank_size = 14
        self.fuel_level = 0
        self.size=size
        self.speed=speed

    def fuel_up(self):
        self.fuel_level = self.fuel_tank_size
        print('Fuel tank is now full.')

    def drive(self):
        print(f'The {self.model} is now driving.')

    def get_size(self):
        print(f"the size of the airplane is {self.size}")

    def get_speed(self):
        print(f"the maximum speed of the airplane is {self.speed}")

    def increase_speed(self):
        self.speed *= 1.1
        print(f"the maximum speed of the airplane is {self.speed}")

class Airbus(Airplane):
    def __init__(self, brand, model, type, size:str, speed):
        super().__init__(brand, model, type, size, speed)
        self.size=size
        self.speed=speed
        self.fuel = FuelStorage("airbus", "A lot", "very fast", "Airplane" )
        self.fuel_level = 0

    def charge_airplane(self, new_value):
        self.fuel.charge_fuel(new_value)
        print('The airplane is now charged.')

    def fuel_up(self):
        print('This airplane has no fuel tank!')

    def decrease_speed(self):
        self.speed *= 0.9
        print(f"the new speed is {self.speed}")

    def get_model(self):
        print(f"the model of the airbus is {self.model}")

    def get_brand(self):
        print(f"the brand of the airbus is {self.brand}")

class FuelStorage:
    def __init__(self, brand, amount, speed_of_fuel, type:str, size:int = 20):
        self.size = size
        self.fuel_level = 0
        self.type=type
        self.speed_of_fuel=speed_of_fuel
        self.amount=amount
        self.brand=brand

    def get_fuel_level(self):

        return self.fuel_level

    def get_amount(self):

        return 10*self.fuel_level

    def charge_fuel(self, new_value):
        self.fuel_level = new_value

    def __repr__(self):
        return f"<This is the fuel> size {self.size} fuel level {self.charge_level}"

    def get_type(self):
        return f"the type of fuel is {self.type}"


vehicle_object = Airplane('Boeing', '747', 'Airplane', 'very big', 988)

my_airbus = Airbus('Airbus', 'a380', 'Airplane', 'extremely big', 1185)
print(my_airbus.fuel.get_fuel_level())
my_airbus.charge_airplane(50)
my_airbus.fuel.charge_fuel(50)
print(my_airbus.fuel.get_fuel_level())
```
![](homework_inheritance_pic)
