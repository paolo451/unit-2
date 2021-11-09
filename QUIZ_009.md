## QUIZ #009

```.py
## This function returns the missing number from a list of numbers

def missingNumber(sorted):
    sort_len = len(sorted) - 1
    z = 0
    for i in range(sorted[0], sorted[sort_len]):
        if sorted[z] != i:
            return i
        z += 1
```

Prove that it works:

![image](https://user-images.githubusercontent.com/88994602/140899814-3ccbec73-15a3-4a10-b16c-e6e48a542f14.png)
