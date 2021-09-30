## In the first exercise, the user enters "Hello" and a booleon. If the booleon is true, the "Hello" turns into "olleh". If the booleon is false, the "Hello" turns into "olleH".
```.py
def mystery_box1(n1, n2):
    len_n1 = len(n1)
    string1 = ""
    if n2 == True:
        n3 = n1.lower()
        for i in range (len_n1 -1, -1, -1):
            string1 += n3[i]
    else:
        for i in range(len_n1 -1, -1, -1):
            string1 += n1[i]
    return string1

out1 = mystery_box1("Hello", True)
print(out1)
```
## In the second exercise, the user enters their email. The code will seperate their name and their email mark.
```.py
def mystery_box2(email):
    name = ""
    length = len(email)
    domain = ""
    name_finish = False
    for i in range(length):
        if email[i] == "@":
            name_finish = True
        if name_finish == True:
            domain += email[i]
        else:
            name += email[i]
    answer = f"{name}" + "            " f"{domain}"
    return answer
out1 = mystery_box2("elia.kobayashi@uwcisak.jp")
print(out1)
```
## In the third exercise, the user enters three numbers. The code will determine the least common multiple for the three numbers.
```.py
def mystery_box3(n1,n2,n3):
    if n1 > n2 and n1 > n3:
        greatest = n1
    elif n2 > n1 and n2 > n3:
        greatest = n2
    elif n3 > n1 and n3 > n2:
        greatest = n3
    while(True):
        if ((greatest % n1 == 0) and (greatest % n2 == 0) and (greatest % n3 == 0)):
            answer = greatest
            break
        greatest += 1
    return answer
output1 = mystery_box3(5,10,7)
print(output1)
```
## In the fourth exercise, the user enters their IB score in each class. The code will determine if any of the inputs are not an IB grade. Additionally, the code will determine the average score.
```.py
def mystery_box4(n1, n2, n3, n4, n5, n6,):
    sum = 0
    division = 0
    list = []
    if n1 <= 7:
        sum += n1
        list.append(n1)
        division += 1
    if n2 <= 7:
        sum += n2
        list.append(n2)
        division += 1
    if n3 <= 7:
        sum += n3
        list.append(n3)
        division += 1
    if n4 <= 7:
        sum += n4
        list.append(n4)
        division += 1
    if n5 <= 7:
        sum += n5
        list.append(n5)
        division += 1
    if n6 <= 7:
        sum += n6
        list.append(n6)
        division += 1
    answer = sum / division
    answer2 = f"{answer}" + "         " + f"{list}"
    return answer2
out= mystery_box4(5, 6, 3, 8, 1, 7,)
print(out)
```
