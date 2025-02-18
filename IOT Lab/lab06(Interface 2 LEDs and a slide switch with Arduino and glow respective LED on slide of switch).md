##Design
![Copy of Lab 6](https://github.com/user-attachments/assets/a94066cc-8896-4998-a139-fcf90eb175c6)
## Code
```
int butt = 7; 
int led1 = 4; 
int led2 = 5;
int reading ; 
void setup() {
  // put your setup code here, to run once:
  pinMode (led1, OUTPUT);
  pinMode (led2, OUTPUT);
  pinMode (butt, INPUT); 
}

void loop() {
  // put your main code here, to run repeatedly:
  reading = digitalRead (butt); 
  if (reading ==1) { 
    digitalWrite (led1, HIGH); 
    delay(500); 
    digitalWrite (led2, LOW); 
    }
  else
  { digitalWrite (led2, HIGH); 
    delay(1000); 
    digitalWrite (led1, LOW); 
    }
    
}
```
