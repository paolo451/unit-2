## QUIZ #020

```.py
## This function converts numbers into scientific notation

def ScientNot(number):
    sci = 0

    while not number < 10:
        number /= 10
        sci += 1

    answ = f"{number} * 1e{sci}"

    return answ

```
**Flowchart:**

![flowhat](https://user-images.githubusercontent.com/88994602/145736382-6e00cb04-c9dc-4ff8-ab06-4a3e5ab0e87c.png)

**Evidence that this works:**

![image](https://user-images.githubusercontent.com/88994602/145736247-dbb217a2-28da-48e8-886e-a5eaa2ee5a72.png)
