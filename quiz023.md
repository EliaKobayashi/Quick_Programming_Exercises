```.py
def odd_numbers(a,b):
    if b >= a:
        answer = "error"
    for i in range(a,b,1):
        if i % 2 != 0:
            print(i)
out = odd_numbers(3,10)
print(out)
```
![](quiz_pic23.png)
