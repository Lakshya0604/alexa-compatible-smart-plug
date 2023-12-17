# alexa-compatible-smart-plug
(Instrument required for making smart plug)

Arduino board


Arduino is a microcontroller-based open source electronic prototyping board which can be programmed with an easy-to-use Arduino IDE.
In this , I will talk about what’s on the Arduino UNO board and what it can do. UNO is not the only board in the Arduino family. There are other boards like Arduino Lilypad, Arduino Mini, Arduino Mega, and Arduino Nano. However, the Arduino UNO board became more popular than other boards in the family because it has documentation that is much more detailed. This led to its increased adoption for electronic prototyping, creating a vast community of electronic geeks and hobbyists.


The major components of Arduino UNO board are as follows:
•	USB connector
•	Power port
•	Microcontroller
•	Analog input pins
•	Digital pins
•	Reset switch
•	Crystal oscillator
•	USB interface chip
•	TX RX LEDs


USB connector

This is a printer USB port used to load a program from the Arduino IDE onto the Arduino board. The board can also be powered through this port.

Power port

The Arduino board can be powered through an AC-to-DC adapter or a battery. The power source can be connected by plugging in a 2.1mm center-positive plug into the power jack of the board.
The Arduino UNO board operates at a voltage of 5 volts, but it can withstand a maximum voltage of 20 volts. If the board is supplied with a higher voltage, there is a voltage regulator (it sits between the power port and USB connector) that protects the board from burning out.

Microcontroller:

It is the most prominent black rectangular chip with 28 pins. Think of it as the brains of your Arduino. The microcontroller used on the UNO board is Atmega328P by Atmel ( a major microcontroller manufacturer). Atmega328P has the following components in it:
•	Flash memory of 32KB. The program loaded from Arduino IDE is stored here.
•	RAM of 2KB. This is a runtime memory.
•	CPU: It controls everything that goes on within the device. It fetches the program instructions from flash memory and runs them with the help of RAM.
•	Electrically Erasable Programmable Read Only Memory (EEPROM) of 1KB. This is a type of nonvolatile memory, and it keeps the data even after device restart and reset.
Atmega328P is pre-programmed with bootloader. This allows you to directly upload a new Arduino program into the device, without using any external hardware programmer, making the Arduino UNO board easy to use.

Analog input pins

The Arduino UNO board has 6 analog input pins, labeled “Analog 0 to 5.” These pins can read the signal from an analog sensor like a temperature sensor and convert it into a digital value so that the system understands. These pins just measure voltage and not the current because they have very high internal resistance. Hence, only a small amount of current flows through these pins.

Although these pins are labeled analog and are analog input by default, these pins can also be used for digital input or output.


Digital pins

You can find these pins labeled “Digital 0 to 13.” These pins can be used as either input or output pins. When used as output, these pins act as a power supply source for the components connected to them. When used as input pins, they read the signals from the component connected to them.
When digital pins are used as output pins, they supply 40 milliamps of current at 5 volts, which is more than enough to light an LED.
Some of the digital pins are labeled with tilde (~) symbol next to the pin numbers (pin numbers 3, 5, 6, 9, 10, and 11). These pins act as normal digital pins but can also be used for Pulse-Width Modulation (PWM), which simulates analog output like fading an LED in and out.

Reset switch

When this switch is clicked, it sends a logical pulse to the reset pin of the Microcontroller, and now runs the program again from the start. This can be very useful if your code doesn’t repeat, but you want to test it multiple times.

Crystal oscillator

This is a quartz crystal oscillator which ticks 16 million times a second. On each tick, the microcontroller performs one operation, for example, addition, subtraction, etc.

USB interface chip

Think of this as a signal translator. It converts signals in the USB level to a level that an Arduino UNO board understands.

TX – RX indicator

TX stands for transmit, and RX for receive. These are indicator LEDs which blink whenever the UNO board is transmitting or receiving data.
Now that you have explored the Arduino UNO board, you have started your journey toward building your first IoT prototype.





