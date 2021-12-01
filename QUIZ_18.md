## QUIZ #18

```.py
## This function outputs the sum of the numbers inputted, except those between the 6 and 7

def sum67(numbers):

    total = 0
    num6 = 0
    num7 = 0

    if 6 in numbers:
        for i in range(len(numbers)):
            if numbers[i] == 6:
                num6 = i

            elif numbers[i] == 7:
                num7 = i

        for x in range(0, num6):
                total += numbers[x]

        for x in range(num7+1, len(numbers)):
                total += numbers[x]
                            
    if not 6 in numbers:
        for i in range(len(numbers)):
            total += numbers[i]
        
    return total

print(sum67([2,2,2,6,9992,7,3])

print(sum67([2,7,2,3]))
```

**Evidence that this works:**

![image](https://user-images.githubusercontent.com/88994602/144288476-27930077-bad4-42a4-b54d-08edefe4d594.png)
