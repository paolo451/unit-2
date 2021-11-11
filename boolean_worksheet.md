## Boolean Worksheet

**1.- Write the logic equation for the diagrams below:**

![image](https://user-images.githubusercontent.com/88994602/141028402-935a8db5-c04d-4a52-9523-0156dbb43278.png)

1.1 - x = AB ⊕ notB

1.2 - x = not(A ⊕ B) * not(A + B)

1.3 - x = not((C + notB) * (B ⊕ A))

1.4 - x = not((B ⊕ C * A ⊕ B) + A ⊕ C)

**2.- Draw the diagram for the logic equations below:**

2.1 - Out1 = A + C + BD + (notB notD)

![image](https://user-images.githubusercontent.com/88994602/141275382-6487dbf8-36bd-4c41-aa74-ff08c04b9a9e.png)

2.2 - Out2 = notB + (notC notD) + CD

![image](https://user-images.githubusercontent.com/88994602/141275403-444a45e5-eaf8-4eee-b6e3-3d24256edf46.png)

2.3 - Out3 = B + notC + D

![image](https://user-images.githubusercontent.com/88994602/141275562-8f8eaf10-dec8-453b-8372-864ec15b80d5.png)

2.4 - Out4 = (notB notD) + (C notD) + (BCnotD) + (notB C) + A

![image](https://user-images.githubusercontent.com/88994602/141275578-0bcede5d-e929-4b56-91c9-b79bd808c786.png)


**3.- Simplify the K-map Tables below and write the logical equations:**

3.1.- 

![image](https://user-images.githubusercontent.com/88994602/141031284-88aa6a4b-5674-4069-8fc7-528e0178d9ec.png)

3.2.- 

![image](https://user-images.githubusercontent.com/88994602/141031861-d04855e8-e53b-4c08-a269-010b053bd984.png)

3.3.- 

![image](https://user-images.githubusercontent.com/88994602/141032099-bfc0c899-01a3-4a5a-8285-413e184a0c31.png)

3.4.- 

![image](https://user-images.githubusercontent.com/88994602/141032522-1e4cf6d2-0b38-4589-a372-385ed1532a85.png)

3.5.- 

![image](https://user-images.githubusercontent.com/88994602/141032925-6c4d306d-7b3c-4eba-a8cb-fbf3d4a7858f.png)

**4.- Find the equation for the notification system for...***

The apartment below needs a notification system  that sends an SMS to the owner when:
a) Any of the two windows is open when the main door is locked,
b) The baranda’s door is open when the main door is locked,
c) The TV screen is ON when the washing machine and the dish washing machine are ON.
Add 2 more rules:
d) The lamp from the living room is on and the TV is off
e) The bathtub is full and the main door is unlocked

Having this basis:

![image](https://user-images.githubusercontent.com/88994602/141282709-2b78616c-83e7-45f8-b119-ffdde1de8481.png)

Given number of variables, and in the sake of practicality, I used the Charlie Coleman K-Map online tool, and inputted the truth table, to get this result:

![image](https://user-images.githubusercontent.com/88994602/141284331-81cec146-a84e-412e-bc3b-f1fcbc99d6a6.png)

Having that, my equation for those 5 different situations turned out to be:

**(notTV x L) + (TV x WM) + (notW x MD) + (notMD x BT) + (MD x notB)**
