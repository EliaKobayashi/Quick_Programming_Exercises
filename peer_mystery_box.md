## Paolo's O's
### Find how many O's are in the input
```.py
def mystery_box(word):
    answer = 0
    for i in range(len(word)):
        if word[i] == "o":
            answer += 1
    return answer
out = mystery_box("Paolo")
print(out)
```
![](hwpic1)
