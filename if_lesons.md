## Minimum of Two Numbers
```.py
Value_a = int(input("please input the value of 'a'"))
Value_b = int(input("please input the value of 'b'"))
if Value_a < Value_b:
    print(Value_a)
else:
    print(Value_b)
``` 
![](1.1_comp.png)   
## Sign Function
```.py
X = int(input("please enter the value for 'X' "))
if X > 0:
    print("1")
elif X == 0:
    print("0")
else: 
    print("-1")    
```
    
## Minimum of three numbers
```.py
Value_a = int(input("please input the value of 'a'"))
Value_b = int(input("please input the value of 'b'"))
Value_c = int(input("please input the value of 'c'"))
if Value_a > Value_b and Value_c > Value_b:
    print(Value_b)
if Value_b > Value_a and Value_c > Value_a:
    print(Value_a)
if Value_a > Value_c and Value_b > Value_c:
    print(Value_c)
```    
 
## Equal Numbers
```.py
Value_a = int(input("please input the value of 'a'"))
Value_b = int(input("please input the value of 'b'"))
Value_c = int(input("please input the value of 'c'"))
if Value_a == Value_c and Value_c == Value_b:
    print("3")
elif Value_a == Value_b or Value_a == Value_c or Value_b == Value_c:
    print("2")
else:
    print("0")
```  
  
## Rook Move
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'd'"))
if a == c or b == d:
    print("YES")
else:
    print("NO")
```


## Chess board: same color
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'd'"))
if (a + b) %2 == 0 and (c + d) %2 == 0:
    print("YES")
elif (a + b) %2 != 0 and (c + d) %2 != 0:
    print("YES")
else:
    print("NO")
```

## Chess board: King move
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'c'"))
if -1<=(a-c)<=1 and -1<=(b-d)<=1:
    print("YES")
else:
    print("NO")
```

## Chess board: Bishop's move
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'c'"))
if abs (a-c) == abs (b-d):
    print("YES")
else:
    print("NO")
```

## Chess board: Queen's move
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'd'"))
if a == c or b == d:
    print("YES")
elif abs (a-c) == abs (b-d):
    print("YES")
else:
    print("NO")
```

## Chess board: Knight's move
```.py
a = int(input("Please input the value of 'a'"))
b = int(input("Please input the value of 'b'"))
c = int(input("Please input the value of 'c'"))
d = int(input("Please input the value of 'd'"))
if abs(a-c)==1 and abs(b-d)==2 or abs(a-c)==2 and abs(b-d)==1:
    print("YES")
else:
    print("NO")
```

## Chocolate bar
```.py
n = int(input("Please input the value of 'n'"))
m = int(input("Please input the value of 'm'"))
k = int(input("Please input the value of 'k'"))
if k < n*m and ((k%n == 0) or (k%m == 0)):
    print("YES")
else:
    print("NO")
```

## Leap Year
```.py
year = int(input("please input the year"))
if year%4 == 0 and year%100 != 0 or year%400 == 0:
    print("LEAP")
else:
    print("COMMON")
```
