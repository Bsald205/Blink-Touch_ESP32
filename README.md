# Blink-Touch_ESP32
Blink en Arduino con touch en ESP32

#include <iostream>

using namespace std;

int x = 15;
int led = 4;

void setup() {
  Serial.begin(115200);
  pinMode (led, OUTPUT);
}

void loop() {
  
  if (digitalRad (x) == HIGH){
    digitalWrite(led, HIGH);
    cout<< "led encendido"<< endl;
  }else {
    digitalWrite(led, LOW);
    cout << "led apagado"<< endl;
  }
  delay (500);
}
