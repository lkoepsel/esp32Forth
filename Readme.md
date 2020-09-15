# espForth

## version 6.5
```
6.5: Changes either due to board (Adafruit ESP32 Feather) or wanting specific 
actions from defined words
Approximate line numbers
60-67: redefined IP to be uint32_t to fix compile error
415: redefined LED_PIN to be 13 for ESP32 Feather
729: redefined DUTY to call ledcWrite to allow for simpler PWM setup
904: changed boot message to 6.5
910: more changes for onboard LED pin 13
951: changed baud rate to 2000000 from 115200

Added primitive words: (See Appendix 2 for details as to how to add a primitive)
?keyt ( -- key ) – test for key entered [if (Serial.available() == 0)]
GTIMM ( -- time ) - get a microsecond time on to stack [micros()]
LED ( level -- ) - set onboard LED high/low [digitalWrite(LED_BUILTIN, level)]
>  ( n1 n2 -- bool ) – set bool to eval of n1 > n2  [>]
IPUN ( pin -- ) - set pin to be an INPUT_PULLUP [pinMode()]
GTIME ( -- time ) - get a millisecond time on to stack [millis()]
DREAD ( pin -- ) - read a digital value on a pin [digitalRead()]
DWRT ( level pin -- ) - set a digital pin high/low [digitalWrite()]
OPIN ( pin -- ) - set pin to be an OUTPUT [pinMode()]
IPIN ( pin -- ) - set pin to be an INPUT [pinMode()]
```

## version 6.2: Original version by CH Ting 
```
Complete Forth Written in C
```

## Author
    Lief Koepsel made edits to espForth 6.2 by CH Ting
    My goal is the same as CH Ting, to use Forth to help students understand 
    Forth and use it to gain a further understanding of working 
    with microcontrollers

    All mistakes made are made by me.
    I appreciate the incredible effort, great documentation and 
    ease of implementation, CH Ting has put into espForth.


## Original Author
    CH Ting
    http://forth.org/OffeteStore/OffeteStore.html

## Purpose of Code
    Use this code along with my Forth class to be published at a later date.


