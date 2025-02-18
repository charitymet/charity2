##Design
![Copy of Lab 7 A SSD](https://github.com/user-attachments/assets/322e2652-974b-4ab8-8a8e-25086d0dea54)
## Code
```
// C++ code
//
int segA = 2;
int segB=3;
int segC=4;
int segD=5;
int segE =6;
int segF=7;
int segG=8;
int i;
void setup()
{ for(i=2;i<9;i++)
  pinMode(i, OUTPUT);
}

void loop()
{
   digit(1,1,1,1,1,1,0);
  delay(200);
  digit(0,0,0,0,0,0,0);
  delay(500);
  
}

void digit(int a,int b,int c,int d,int e,int f, int g)
{
  digitalWrite(segA,a);
  digitalWrite(segB,b);
  digitalWrite(segC,c);
  digitalWrite(segD,d);
  digitalWrite(segE,e);
  digitalWrite(segF,f);
  digitalWrite(segG,g);
}
```
