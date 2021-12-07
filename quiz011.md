```.py
def samefirstlast(list):
    a="False"
    if len(list)>1:
        if list[0]==list[-1]:
            a="True"
    return a
a=samefirstlast([1,2,3,1])
print(a)
```
![](quizpic11.png)
![](flow_diagram11)
