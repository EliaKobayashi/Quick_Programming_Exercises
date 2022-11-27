```.py
import pyfirmata
from pyfirmata import Arduino
import serial
import time
import time
from matplotlib import pyplot as plt

arduino = serial.Serial('/dev/cu.usbserial-10',baudrate=9600,timeout=1)#port of the arduino
def read():
    data=""
    while len(data)<1:
        data=arduino.readline()
    return data

num_temperature = []
num_humidity = []
num_time = []
action = False
desired=60
for a in range(10000):
    time.sleep(0.1)
    value=read()
    msg=value.decode("utf")
    msg=msg.strip()
    messages = msg.split(" ")
    if "Hello" not in messages:
        humidity=messages[0].split(":")[1]
        temperature=messages[1].split(":")[1]
        for i in humidity:
            if i == "%":
                humidity = humidity.replace("%","")
        for x in temperature:
            if x == "C":
                temperature = temperature.replace("C","")
        humidity = float(humidity)
        temperature = float(temperature)
        if action == True:
            Action = 'OFF'
        else:
            Action = 'On'
        if Action == 'Off':
            color=" \033[0;34m"
        else:
            color=" \033[0;31m"
        print(f"Iteration: {a} Desired: {desired} Error: {desired-temperature} Temperature: {temperature} Humidity: {humidity} {color}Action:{Action} \033[00m")
        num_humidity.append(humidity)
        num_temperature.append(temperature)
        num_time.append(a)
        if temperature >= desired:
            print("Temperature is 60")
            action = True
            break

print(num_humidity)
print(num_temperature)
plt.plot(num_time,num_temperature,color="#caf0f8")
plt.show()
plt.plot(num_time,num_humidity,color="#caf0f8")
plt.show()
```
