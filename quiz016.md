## For each pair of characters of an input String, swap every two characters. 
```.py
def CharacterSwap(input):
    answer = ""
    for i in range(1,len(input), 2):
        answer += input[i]
        answer += input[i-1]
    return answer
out = CharacterSwap("ErrorsShould")
print(out)
```
![](quiz_pic16..png)
