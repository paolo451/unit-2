## Code in C for the Project:

Updated to 15/12/2021, only in draft, doesn't have full functionality yet


```.c
char stringToMorseCode[] = "1234567890";

int led12 = 12;      // blink an led on pin 12
int motorPin = 8;      // vibrate thingy on pin 8


// All speeds depend on morse dot, adjusting it to adjust all

int dotLen = 250;     // length of the morse code 'dot'
int dashLen = dotLen * 3;    // length of the morse code 'dash'
int elemPause = dotLen;  // length of the pause between elements of a character
int Spaces = dotLen * 3;     // length of the spaces between characters
int wordPause = dotLen * 7;  // length of the pause between words

void setup() {
  pinMode(led12, OUTPUT);
  pinMode(motorPin, OUTPUT);
  MorseCode();
}

void loop(){
  
}

void MorseCode(){
  for (int i = 0; i < sizeof(stringToMorseCode) - 1; i++)
  {
    // Get the character in the current position
    char tmpChar = stringToMorseCode[i];
    // Set the case to lower case
    tmpChar = toLowerCase(tmpChar);
    // Call the subroutine to get the morse code equivalent for this character
    GetChar(tmpChar);
    delay(1000);
  }
}

// DOT
void MorseDot(){
  digitalWrite(led12, HIGH);    
  digitalWrite(motorPin, HIGH);
  delay(dotLen);              
}

// DASH
void MorseDash(){
  digitalWrite(led12, HIGH);    
  digitalWrite(motorPin, HIGH);  
  delay(dashLen);               
}

// Turn Off
void LightsOff(int delayTime){
  digitalWrite(led12, LOW);     
  digitalWrite(motorPin, LOW);
  delay(delayTime);             
}

// *** Characters to Morse Code Conversion *** //
void GetChar(char tmpChar){
  switch (tmpChar) {
    case '1':
      MorseDot();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      break;
    case '2':
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      break;
    case '3':
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      break;
    case '4':
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      MorseDot();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      break;
    case '5':
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      break;
    case '6':
      MorseDash();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      break;
    case '7':
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      break;
    case '8':
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      MorseDot();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      break;
    case '9':
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      MorseDash();
      LightsOff(elemPause);
      MorseDot();
      LightsOff(elemPause);    
      break;
    case '0':
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      MorseDash();
      LightsOff(elemPause);
      MorseDash();
      LightsOff(elemPause);    
      break;
    default:
      LightsOff(Spaces);
  }
}


``` 
