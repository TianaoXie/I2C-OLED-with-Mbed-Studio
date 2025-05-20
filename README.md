To use this library, you should add **#include "i2c_oled.h"** in your c/cpp file.

Here is a demo for this library.
```
#include "mbed.h"
#include "i2c_oled.h"

int main() {
  ThisThread::sleep_for(100);
  OLED_Init();
  while (true) {
        OLED_ShowNum(1, 1, 1001, 4); // Start from row 1 column 1, show a number 1001 whose length is 4.
        OLED_ShowString(2, 1, "Jason Wu"); // Start from row 2 column 1, show a string "Jason Wu".
        OLED_ShowSignedNum(3, 1, -12, 2); // Start from row 3 column 1, show a signed number -12 whose length is 2.
  }
}
```
