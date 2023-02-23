``` c
#include <Arduino.h>


float measurement = 0;
void setup() {
  // put your setup code here, to run once:
  Serial.begin(115200);
  
}

void loop() {
  
  

    measurement = temperatureRead();
 
    Serial.print("Hall sensor measurement: ");
    Serial.println(measurement); 
 
    delay(1000);

}
```