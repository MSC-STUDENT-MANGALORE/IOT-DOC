# IOT-DOC
1.https://wokwi.com/projects/333796636268429907
2.https://wokwi.com/projects/333797944251646547
3.https://wokwi.com/projects/333801274561528403
4.https://wokwi.com/projects/333806173307273812
5.https://wokwi.com/projects/334346714953548371 temperature and humidity

https://www.electronicshub.org/dht11-humidity-sensor-arduino/
https://lastminuteengineers.com/dht11-dht22-arduino-tutorial/

Ultrasonic Sensor
https://wokwi.com/projects/334344881532043858

PIR sensor:
https://wokwi.com/projects/334346049182237266

temperature and humidity:
https://wokwi.com/projects/334346714953548371 temperature and humidity


int sensorPin = A0; 
int sensorValue;  
int limit = 300; 

void setup() {
 Serial.begin(9600);
 pinMode(13, OUTPUT);
}

void loop() {

 sensorValue = analogRead(sensorPin); 
 Serial.println("Analog Value : ");
 Serial.println(sensorValue);
 
 if (sensorValue<limit) {
 digitalWrite(13, HIGH); 
 }
 else {
 digitalWrite(13, LOW); 
 }
 
 delay(1000); 
}
