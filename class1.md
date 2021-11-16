```.c
// Not quite sure what this is supposed to do...
// Something like an average?

void setup()
{
  Serial.begin(9600); 
  
  int test2 [6] = {5,7,9,1,7,10};
  Serial.println("Shokin result is");
  Serial.println(shokin(test2));
}

float shokin(int nums[]){
  uint8_t N = sizeof(nums)/sizeof(uint8_t);
  float average = 0.0;
  
  for (int i = 0; i < N - 3; i++){
  average += (nums[i] + nums[i+1] + nums[i+2]) / 3;
  }  
  return average;
}

void loop()
{
  
}

```
