# IOT25_HW03

#사진
![assignment3_screenshot](assignment3_screenshot.jpg)

#영상
![assignment3_video](assignment3_video.mp4)

#실행 코드
'''arduino
// Potentiometer is connected to GPIO 34 (Analog ADC1_CH6) 
const int potPin = 34;

// variable for storing the potentiometer value
int potValue = 0;

void setup() {
  Serial.begin(115200);
  delay(1000);
}

void loop() {
  // Reading potentiometer value
  potValue = analogRead(potPin);
  Serial.println(potValue);
  delay(500);
}
