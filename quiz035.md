```.py
''' 
A programme to calculate number of matches Lily needs to use to eescape the tiger
'''
class Lily:
    def __init__(self, meters, seconds):
        self.meters=meters
        self.seconds=seconds

''' calculation to figure out the answer '''

    def matchsticks(self):
        import math
        seconds2 = self.seconds / 100
        answer = self.meters / seconds2 / 5
        return math.ceil(answer)

out = Lily(250,110)
print(out.matchsticks())
```
![](quiz_pic35.png)
