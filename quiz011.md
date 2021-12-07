```.py
def samefirstlast(list):
    a="False"
    if len(list)>1:
        if list[0]==list[-1]:
            a="True"
    return a
a=samefirstlast([1,2,3,1])
print(a)
b=samefirstlast([1,2,3])
print(b)
```
![](quizpic11.png)
![](flow_diagram11)
