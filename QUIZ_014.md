## QUIZ #014

```.py
def evenlySpaced(a,b,c):
    numbers = []
    res = False

    numbers.extend([a,b,c])
    numbers.sort()

    if numbers[1] - numbers[0] == numbers[2] - numbers[1]:
        res = True

    return res
```


**Evidence that this works**

![image](https://user-images.githubusercontent.com/88994602/144290318-4d776f55-2788-47e8-b7ec-0f76e0fa646c.png)
