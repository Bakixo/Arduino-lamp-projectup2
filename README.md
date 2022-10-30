# Arduino-lamp-projectup2
second development of my first project





int buton = 8;
int led = 10;
int butonDurum;
 
void setup() {
  pinMode(led, OUTPUT);
  pinMode(buton, INPUT); 
}
 
void loop() {
  butonDurum = digitalRead(buton); 
  delay(100);
  if (butonDurum == 1) {
    digitalWrite(10,!digitalRead(led));
  }
}
