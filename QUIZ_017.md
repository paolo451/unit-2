## QUIZ #017

```.py
## This function outputs True if you can make a triangle with the inputted numbers as size of the sides

def triangle(a,b,c):

    res = False

    if a+b>c and a+c>b and b+c>a:
        res = True

    return res
```

**Evidence that this works:**

![image](https://user-images.githubusercontent.com/88994602/144291139-e1d19dd3-7798-418a-9afb-2de9241e2441.png)
