## QUIZ #013:

```.py
## This function gets the total cost of a list of products, taking into consideration the tax according to its type. 
## If the type of a certain product isn't included in the database, it allows for it to be inputted manually

def cost(items, prices):

    food = ["BREAD", "PIZZA", "RICE"]
    elect = ["IPAD", "CELLPHONE", "LAPTOP"]
    liq = ["BEER", "VODKA", "RUM"]

    total = 0

    for i in range(0, len(items)):
        if items[i].upper() not in food and items[i].upper() not in elect and items[i].upper() not in liq:

            p_type = input(f"We don't have {items[i].upper()} in our database. Please input its type. (Food, Electronics, or Liquor)").upper()

            if p_type == "LIQUOR":
                liq.append(items[i].upper())

            elif p_type == "FOOD":
                food.append(items[i].upper())

            elif p_type == "ELECTRONICS":
                elect.append(items[i].upper())

        if items[i].upper() in food:
            total += prices[i] * 1.1

        if items[i].upper() in elect:
            total += prices[i] * 1.15

        if items[i].upper() in liq:
            total += prices[i] * 1.2            

    return total
```

### Prove that this works:

![image](https://user-images.githubusercontent.com/88994602/142574480-28bbc211-bc84-4490-b2dd-55ef53b2c62e.png)
