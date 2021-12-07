## Given an array of numbers, output TRUE if the array is length 1 or more, and the first element and the last element are equal. Otherwise output FALSE.
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
![](quiz_pic11.png)
![](flow_diagram11)
