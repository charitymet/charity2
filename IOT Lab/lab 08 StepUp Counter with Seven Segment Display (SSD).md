##Design
![Copy of Lab 7 A SSD (1)](https://github.com/user-attachments/assets/0399747c-1d77-4c27-a6f4-3b4e3c90d33e)
##Code
```
int segA = 2;
int segB = 3;
int segC = 4;
int segD = 5;
int segE = 6;
int segF = 7;
int segG = 8;
int i;

void setup() {
  for(i = 2; i < 9; i++)
    pinMode(i, OUTPUT);
}

void loop() {
  for(int num = 1; num <= 9; num++) {
    displayDigit(num);
    delay(1000); // Wait for 1 second between numbers
  }
}

void displayDigit(int num) {
  // Map the number to the corresponding segments (A-G)
  switch(num) {
    case 1:
      digit(0, 1, 1, 0, 0, 0, 0);  // Segments BC
      break;
    case 2:
      digit(1, 1, 0, 1, 1, 0, 1);  // Segments ABDEG
      break;
    case 3:
      digit(1, 1, 1, 1, 0, 0, 1);  // Segments ABCDG
      break;
    case 4:
     digit(0, 1, 1, 0, 0, 1, 1);  // Segments BCFG
      break;
    case 5:
      digit(1, 0, 1, 1, 0, 1, 1);  // Segments ACDFG
      break;
    case 6:
      digit(1, 0, 1, 1, 1, 1, 1);  // Segments ACDEFG
      break;
    case 7:
      digit(1, 1, 1, 0, 0, 0, 0);  // Segments ABC
      break;
    case 8:
      digit(1, 1, 1, 1, 1, 1, 1);  // Segments ABCDEFG
      break;
    case 9:
      digit(1, 1, 1, 1, 0, 1, 1);  // Segments ABCDFG
      break;
    default:
      // Default case (clear the display)
      digit(0, 0, 0, 0, 0, 0, 0);
  }
}

void digit(int a, int b, int c, int d, int e, int f, int g) {
  digitalWrite(segA, a);
  digitalWrite(segB, b);
  digitalWrite(segC, c);
  digitalWrite(segD, d);
  digitalWrite(segE, e);
  digitalWrite(segF, f);
  digitalWrite(segG, g);
}
```
