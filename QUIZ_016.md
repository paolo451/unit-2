## QUIZ #016

```.py
## This function returns the inputted word inverting characters 2 by 2

def reversed(word):
    answ = ""

    for i in range(1,len(word),2):
        answ += word[i]
        answ += word[i-1]

    return answ
```

**Evidence that this works**

![image](https://user-images.githubusercontent.com/88994602/144292320-3b1a5504-33ec-4f10-a601-ad0ac918c601.png)
