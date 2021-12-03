## QUIZ #019

```.py
## This function returns the ways a number can be mirrored in a time format

def MirroredTime(n):
    answ = []

    if n >= 24:
        answ.append("NONE")

    if n < 24:
        answ.append(f"{n}:{n}")

        inv = str(n)[::-1]
        if int(inv) < 60 and not f"{n}:{inv}" in answ:
            answ.append(f"{n}:{inv}")

    return answ
```

**Evidence that this works**
![image](https://user-images.githubusercontent.com/88994602/144557217-66a6e623-f903-40e1-81fb-7109b7679b3b.png)

