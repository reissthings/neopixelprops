#Neopixel props ;
Implementing neopixels in props and shit people don't tell you online
-----------------------------------------------------------------------------------------------
1. **Understanding the circuit**
In a neopixel circuit, we have :
- [1] Neopixel Strips (WS2812B)
- [2] Arduino (Nano or pro mini)
- [3] Capacitor, Resistors , buttons and switches
- [4] Wires
- [5] Batteries (Which usually amount to 3.7, sometimes 9V/12V)
- [6] of course, soldering materials

>Neopixels runs at 5V and a maximum of 60mA per LED, although we rarely hit that stage. The data input has to be around 5V± and they can be _*shared between 2 different strips*_(SURPISEEEEEE). They run off the power supply of the arduino (NOT THE 5V PIN). They come in different lengths between each LEDs, so be sure to know what you need otherwise your prop will look like it has hypertelorism.
----------------------
>Ever get confused about batteries by cosplayers trying to make things easy saying shit like : "hur dur lipo batteries lipo this lipo that"? Well you don't need to worry anymore, because I am here to tell you to just use _18650 batteries_. Majority of the so called "lipo battery packs" literally consists of this 18650, and _*THEY APPEAR IN MANY POWERBANKS*_ as well. Before anyone points out that 18650 are Li-ion, yes i am aware but some people on youtube calls it "lipo" LMAO
- Let's get abit logical. People tell you to use powerbanks because it's convenient and it gives off 5V. HOWEVER, 18650 Batteries which appears in powerbanks, are rated at 3.7V. What is the thing that turns the 3.7V into a 5V? ........ There's a module in there that converts/step up the voltage to 5V. These modules can be found under "powerbank modules" or boost converter. Personally, I use the TP4056 with boost converter (or J5019) as it charges the battery and outputs 5V. No more expensive 500C/100C POWERBOOST bullshit! More importantly, no more unnecessary weight your props are dying to support!
- *But @reissthings, what about those flat lipo batteries that looks like it can cause mass destruction?* /// Well, those batteries are rated at 3.7V too. They work the same way as the 18650, really. See what's convenient for you.
>Capacitor and resistors are there just to protect the circuit from sudden jump of current. Capacitors are connected parallel to the powersupply to the Neopixels. Resistor is connected in series from the Data pin of the Arduino to ----> Data pin of the Neopixel strip. Switches are there to.... well, switch on and switch off shit. Buttons are optional, but they allow us to cycle different animations of the neopixel by pushing the button.
-
> The Arduino in props are usually either pro mini or nano, sometimes trinket if you're super rich. But since budget are of the essence, grab an arduino nano/mini from aliexpress/taobao. These arduinos contain CH340G chips, which you have to download a driver in order for it to work. 
