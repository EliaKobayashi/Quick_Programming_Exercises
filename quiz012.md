```.py
def SameFirstLast(array):
    first_num = array[0]
    last_num = array[len(array) -1]
    if len(array) > 1:
        if first_num == last_num:
            answer = True
        else:
            answer = False
    else:
        answer = False
    return answer
```
![](quiz_pic012.png)
