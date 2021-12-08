## QUIZ #011

```.py
# This function returns true if the inputted list is longer or equal than 1 
# and has the same first and last element

def SameFirstLast(numbs):
    answ = False
    leng = len(numbs)

    if leng >= 1 and numbs[0] == numbs[leng-1]:
        answ = True

    return answ
``` 

**Evidence that this works:**

![image](https://user-images.githubusercontent.com/88994602/141428466-cd4d682e-548b-4108-8ec5-525aa0af5c4b.png)

**Flowchart**

![quiz011](https://user-images.githubusercontent.com/88994602/145294256-ec66ba6d-05d2-41cd-a7e3-3372dd2e4920.png)
