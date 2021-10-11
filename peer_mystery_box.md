## Paolo's O's
```.py
def mystery_box(word):
    # How many O's are in the input
    answer = 0
    for i in range(len(word)):
        if word[i] == "o":
            answer += 1
    return answer
out = mystery_box("Paolo")
print(out)

```
![](hwpic1.png)
