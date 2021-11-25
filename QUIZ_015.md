## QUIZ #015

```.py
## This program turns an input like "010!011!000" into its corresponding 
## decimal equivalent, where the exclamation indicates to start over the conversion

def reverseMM(numbs):
    answ = []
    prog = numbs.split("!")

    for i in range(3):
        binnum = prog[i]
        exponent = 1
        res = 0

        for digit in binnum[::-1]:
            res += int(digit) * exponent
            exponent *= 2

        answ.append(str(res))
        
    return "".join(answ)
```
**Prove that this works**

![image](https://user-images.githubusercontent.com/88994602/143484668-7860cb45-89cb-447e-a560-71d4c0029f6f.png)

