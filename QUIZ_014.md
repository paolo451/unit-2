## QUIZ #014

```.py
## This function outputs True if the inputted numbers are evenly spaced

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

**Flowchart:**

![quiz014](https://user-images.githubusercontent.com/88994602/145294102-fa59bb00-b8b1-4767-89f8-8c372db90cbd.png)
