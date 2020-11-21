# BasicArduino
 The follwing files are my second foray into Arduino
 
 
## Table of Contents
* [Table of Contents](#TableOfContents)
* [LED_Fade](#LED_Fade)
* [HelloFunctions](#HelloFunctions)
* [NewPing](#NewPing)
---

## LED_Fade

### Description & Code
 Instead of just blinking, you can make the led slowly change brightness, causing it to fade. 


```C++
//Ellen Lynch
//November 18, 2020
//This code makes the led fade. 

// the loop routine runs over and over again forever:
void loop() {
  // set the brightness of pin 9:
  analogWrite(led, brightness);

  // change the brightness for next time through the loop:
  brightness = brightness + fadeAmount;

  // reverse the direction of the fading at the ends of the fade:
  if (brightness <= 0 || brightness >= 255) {
     fadeAmount = -fadeAmount;
     
  }
  
  delay(30);   // wait for 30 milliseconds to see the dimming effect
}
```

Talk about how the fade works, here....
Fading is different than blinking an led because the brightness is going from the minimum to maximum (0-255) in incrememnts of 5 and repeats. The higher the delay number is, the longer the fade will take and it will look less like a fade and more like the led is just lighting up and then sometimes going out. 

### Evidence
[LED Fade on Arduino Create](https://create.arduino.cc/editor/helmstk1/9e044cca-43d7-4d93-885f-e6dec5b4f769/preview)

### Images
![Fade](Fade Arduino.jpg)
Credit to [magiceco](https://fritzing.org/projects/led-fade-by-magiceco)
### Reflection

## HelloFunctions

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection

## NewPing

### Description & Code
Description goes here

Here's how you make code look like code:

```C++
Code goes here
```
Talk about how the code works, here....

### Evidence
link goes here

### Images
draw it yourself, take a picture, make a fritzing, whatever you want to EFFECTIVELY communicate how its put together.

### Reflection

