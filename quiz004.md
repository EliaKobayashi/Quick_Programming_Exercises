```.py
def perfectN(n = int):
  '''
  Function to divide an integer to its functions
  '''
    answer = []
    for i in range(1, n):
        if n % i == 0:
            answer.append(i)
    return answer
output = perfectN(n = 6)
print(output)
```
![](quiz_pic04)
