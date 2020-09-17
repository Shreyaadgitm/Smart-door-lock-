# Smart-door-lock-

#include<Servo.h>
Servo servo;
int pos=0;
void setup()
{
  pinMode(7, INPUT);
  servo.attach(11);
 
  
  
}

void loop()
{
  if(digitalRead(7)== HIGH)
  {
    servo.write(90);
    delay(500);
    servo.write(180);
    delay(500);

 
     
  }
}