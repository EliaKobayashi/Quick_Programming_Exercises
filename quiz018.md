```.py
def array(num):
    answer = 0
    counter = 0
    flag = True
    while counter < len(num):
        if num[counter] == 6:
            flag = False
        if flag == True:
            answer += num[counter]
        if num[counter] == 7:
                flag = True
        counter += 1
    return answer
out = array([1,2,6,99,7])
print(out)
```
![](quiz_pic18.png)
