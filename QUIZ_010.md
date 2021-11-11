## QUIZ #010
```.py
## This function gives the biggest difference between two neighbouring numbers

def bigNeighbour(numbs):
    answ = 0

    for i in range(1, len(numbs)):
        if numbs[i] - numbs[i-1] > answ:
            answ = numbs[i] - numbs[i-1]

    return answ
```

**Prove that it works:**

![image](https://user-images.githubusercontent.com/88994602/141215149-4558b1fc-5dc5-4c9d-9e5d-77149e99e7e3.png)
