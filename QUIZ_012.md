## QUIZ #012
```.py

## This function returns the average length of the words inputted as a list

def wordlength(words):
    leng = 0

    for i in range(0, len(words)):
        leng += len(words[i])    
    leng /= len(words)         

    return leng

``` 

Prove that this works:

![image](https://user-images.githubusercontent.com/88994602/142161290-c15cecdf-22b5-4a06-8706-c6325f868d47.png)
