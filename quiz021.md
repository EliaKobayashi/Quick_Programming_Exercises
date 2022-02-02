```.py
def ScientificNotation(num):
    num1 = str(num)
    num2 = len(num1) - 1
    answer = f"{num1[0]}.{num1[1]}{num1[2]} * 1e{num2}"
    return answer
out = ScientificNotation(132000)
print(out)
```
![](quiz_pic21.png)
