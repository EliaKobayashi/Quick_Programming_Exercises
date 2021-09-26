### Ask the user for  2 numbers, A and B, Output TRUE if one of them is 10 or if their sum is 10.
```.py
a = int(input("Please enter the first number: "))
b = int(input("Please enter the second number: "))
if a == 10:
    print("True")
elif b == 10:
    print("True")
elif a + b == 10:
    print("True")
else:
    print("False")
```
