## QUIZ #021

```.py
## This function returns the hour it must be for a clock to show the inputted number of degrees

def circle(degrees):
    hours = degrees // 30
    minutes = degrees % 30
    ang_minutes = minutes*2

    if ang_minutes == 0:
        ang_minutes = "00"

    answ = f"{hours}:{ang_minutes}"
    
    return answ
```

**Flowchart:**

![gaaa](https://user-images.githubusercontent.com/88994602/145736995-be82026e-6a8d-4ecb-bc65-f3fb2420222f.png)

**Evidence that this works:**

![image](https://user-images.githubusercontent.com/88994602/145737033-d675e9c3-a0ea-4300-8a08-e2e84282b2ee.png)
