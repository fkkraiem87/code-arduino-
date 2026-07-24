# Arduino Button With LED 🔘💡

## Description

This project explains how to control an LED using a push button with Arduino.

When the button is pressed, Arduino detects the signal and turns the LED ON.
When the button is released, the LED turns OFF.

This is a simple project to learn how Arduino reads inputs from components and controls outputs.

## Components

* Arduino UNO
* Push button
* LED
* 220Ω resistor (for LED)
* 10kΩ resistor (for button)
* Breadboard
* Jumper wires

## How It Works

The button is connected to an Arduino input pin. Arduino continuously checks the button state.

* Button pressed → Arduino receives `HIGH` → LED turns ON.
* Button released → Arduino receives `LOW` → LED turns OFF.

The LED is connected to an output pin, so Arduino can control when it lights up.

## Main Arduino Functions Used

### `pinMode()`

Used to define if a pin is an input or an output.

Example:

```cpp
pinMode(buttonPin, INPUT);
pinMode(ledPin, OUTPUT);
```

* The button pin is an **INPUT** because Arduino reads its signal.
* The LED pin is an **OUTPUT** because Arduino controls it.

### `digitalRead()`

Used to read the button state.

Example:

```cpp
buttonState = digitalRead(buttonPin);
```

It gives:

* `HIGH` → button pressed
* `LOW` → button not pressed

### `digitalWrite()`

Used to control the LED.

Example:

```cpp
digitalWrite(ledPin, HIGH);
```

* `HIGH` → LED ON
* `LOW` → LED OFF

## Project Result

After uploading the code:

* Pressing the button lights the LED.
* Releasing the button turns the LED off.

This project is a first step to understanding how Arduino uses **inputs** (buttons, sensors) to control **outputs** (LEDs, motors, displays).
