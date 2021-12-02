## Automatic Counter (4-bits)

### The code:
```.c
// This is an automatic counter for four bits

void setup(){
Serial.begin(9600);
  
  bool bit0 = 1;
  bool bit1 = 1;
  bool bit2 = 1;
  bool bit3 = 1;
  
  for(int q = 0; q < 2; q++){
    bit3 = !bit3;
  
    for(int z = 0; z < 2; z++){    
      bit2 = !bit2;

        for(int j = 0; j < 2; j++){    
          bit1 = !bit1;

            for(int i = 0; i < 2; i += 1){
            bit0 = !bit0;

            Serial.print("\n\n Bit 3 is: ");            
            Serial.print(bit3);          
            Serial.print("\n Bit 2 is: ");            
            Serial.print(bit2);
            Serial.print("\n Bit 1 is: ");
            Serial.print(bit1);
            Serial.print("\n Bit 0 is: ");
            Serial.print(bit0);   
        }
      }
    }
  }
  
}

void loop(){
}
```

### The Arduino Setup

(This was previously set-up as a seven segment display counter, however, it's not necessary for the counter to work)

![image](https://user-images.githubusercontent.com/88994602/144484844-5e942ba9-9bb3-4d94-b8ad-e3ff54af1ee6.png)


### Output

![image](https://user-images.githubusercontent.com/88994602/144484944-b6c1ac5c-481a-40a7-9853-489e6a980577.png)
