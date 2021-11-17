## Binary Counter

### Circuit

![image](https://user-images.githubusercontent.com/88994602/141967870-f0cf07b6-6a10-4f91-bbf9-05f5cba5a807.png)

### Code

 ```.c
int pin3 = 3;
int pin4 = 4;
int pin5 = 5;
int waitTime = 1000;
  

void setup(){
  pinMode(pin3, OUTPUT);
  pinMode(pin4, OUTPUT);
  pinMode(pin5, OUTPUT);

}

void loop(){
  digitalWrite(pin3, LOW);
  digitalWrite(pin4, LOW);
  digitalWrite(pin5, LOW);  
  delay(waitTime);
    
  digitalWrite(pin3, LOW);
  digitalWrite(pin4, LOW);
  digitalWrite(pin5, HIGH);  
  delay(waitTime);
    
  digitalWrite(pin3, LOW);
  digitalWrite(pin4, HIGH);
  digitalWrite(pin5, LOW);  
  delay(waitTime);    
  
  digitalWrite(pin3, LOW);
  digitalWrite(pin4, HIGH);
  digitalWrite(pin5, HIGH);  
  delay(waitTime);    
  
  digitalWrite(pin3, HIGH);
  digitalWrite(pin4, LOW);
  digitalWrite(pin5, LOW);  
  delay(waitTime); 
    
  digitalWrite(pin3, HIGH);
  digitalWrite(pin4, LOW);
  digitalWrite(pin5, HIGH);  
  delay(waitTime); 
    
  digitalWrite(pin3, HIGH);
  digitalWrite(pin4, HIGH);
  digitalWrite(pin5, LOW);  
  delay(waitTime);    
    
  digitalWrite(pin3, HIGH);
  digitalWrite(pin4, HIGH);
  digitalWrite(pin5, HIGH);  
  delay(waitTime);    
}
 ```
## Circuit for the number you want

![image](https://user-images.githubusercontent.com/88994602/142127586-7469fe0a-9ec9-4495-9e24-828ae0e18a43.png)

Here the image shows that when switches #1 and #3 are on, the leds display 101, in representation of number 5

## Code for the number you want

```.c
int pin3 = 3;
int pin4 = 4;
int pin5 = 5;
  

void setup(){
  pinMode(pin3, OUTPUT);
  pinMode(pin4, OUTPUT);
  pinMode(pin5, OUTPUT);
  
  digitalWrite(pin3, HIGH);
  digitalWrite(pin4, HIGH);
  digitalWrite(pin5, HIGH);  
}

void loop(){
}
```
