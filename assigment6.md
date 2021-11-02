# Lab 6: YOUR_FIRSTNAME FAMILYNAME

Link to your `Digital-electronics-2` GitHub repository:

https://github.com/gondocal99/digital-electronics-2/new/main


### LCD display module

1. In your words, describe what ASCII table is.
   * ASCII is a way of storing numbers, letters, or symbols for exchanging information between computer systems.

2. (Hand-drawn) picture of time signals between ATmega328P and LCD keypad shield (HD44780 driver) when transmitting three character data `De2`.

   
![IMG_6836](https://user-images.githubusercontent.com/91128808/139805848-5c70675d-4549-4b64-b4a2-49f55e7a1968.jpg)


### Stopwatch

1. Flowchart figure for `TIMER2_OVF_vect` interrupt service routine which overflows every 16&nbsp;ms but it updates the stopwatch LCD approximately every 100&nbsp;ms (6 x 16&nbsp;ms = 100&nbsp;ms). Display tenths of a second and seconds `00:seconds.tenths`. Let the stopwatch counts from `00:00.0` to `00:59.9` and then starts again. The image can be drawn on a computer or by hand. Use clear descriptions of the individual steps of the algorithms.

   ![your figure]()


### Custom characters

1. Code listing with syntax highlighting of two custom character definition:

```c
/* Variables ---------------------------------------------------------*/
// Custom character definition
uint8_t customChar[16] = {
   0b10001,
   0b01010,
   0b00100,
   0b00100,
   0b01110,
   0b10001,
   0b01010,
   0b00100,
   0b10001,
   0b01010,
   0b00100,
   0b00100,
   0b01110,
   0b10001,
   0b01010,
   0b00100

};
```


### Kitchen alarm

Consider a kitchen alarm with an LCD, one LED and three push buttons: start, +1 minute, -1 minute. Use the +1/-1 minute buttons to increment/decrement the timer value. After pressing the Start button, the countdown starts. The countdown value is shown on the display in the form of mm.ss (minutes.seconds). At the end of the countdown, the LED will start blinking.

1. Scheme of kitchen alarm; do not forget the supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values.

  ![image](https://user-images.githubusercontent.com/91128808/139804515-c60110b8-f892-4a8c-9b68-48a9d58f4582.png)

