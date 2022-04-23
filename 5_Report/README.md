Introduction
The project is based on microcontroller . Automatic traffic signal helps in fast and efficient control. It helps in smooth management of the traffic control process and tracking the overall operations. In the project, controller used is ATmega 328p which performs and controls the working of the model. In order to display the status, 16×2 Liquid crystal display is used. This  greatly reduce the human effort to control the traffic.  These are produced with secure manufacturing practices, and by design, are selfcontained, battery-powered and lack any networking capability. 

OBJECTIVES 
 The design and implementation is divided into different objectives and outcomes. Below are the list of objectives- 
•	To generate the automatic traffic signal

COMPONENT ANALYSIS 
ATmega 328p 
ATmega328P is high performance, low power controller from Microchip. ATmega328P is an 8-bit microcontroller based on AVR RISC architecture. It is the most popular of all AVR controllers as it is used in ARDUINO boards. It has 14 digital I/O pins, of which 6 can be used as PWM outputs and 6 analog input pins. 
These I/O pins account for 20 of the pins. 
The pinout for the Atmega328 is shown below- 
![image](https://user-images.githubusercontent.com/68462123/164845964-24158a7e-5432-416e-abdf-52955b151c1f.png)

HD44780 LCD 
In the 1980s, Hitachi developed the HD44780 LCD controller, a Dot matrix liquid crystal display (LCD) controller with alphanumeric digits. The controller's character set contains ASCII characters, Japanese Kana characters, and some symbols in two 28-character lines. 
![image](https://user-images.githubusercontent.com/68462123/164846206-f71c5577-896b-4104-8533-4dc68ad6604f.png)
a spring) returns the switch to its default position, restoring the initial condition of the circuit. 

Working and Methodology 
Initially, the user has to move close to the sensing region of the PIR sensor which primarily detects the motion. Note that in Simulide simulation, switch pulled up to 5V is used to mimic the sensor. Whenever the motion is detected, corresponding high signals are fed to the controller. The switch is connected to the digital pin of the IC.  
The LCD initially shows the greeting messages. As the switch is on( indicating motion detected), blinking of the green LED starts along with the message written to the display “Please cast your valuable vote”. The register select, enable and register write pins of LCD is connected to pin 5,7 and 6 respectively of PORTD of the IC. The data pins D4 –D7 is connected to B4 – B7 digital pins of IC respectively. The LCD display operates in 4 bit mode. 
The “lcdcmd” function sends the necessary commands for initialization in 4 bit mode. The “lcd_init” initializes the LCD and the “lcddata” function sends the string data to the LCD to which strings are passed by the lcd_print function. “sei” is used to initialize the all the global flags. 

RESULTS AND CONCLUSION
![image](https://user-images.githubusercontent.com/68462123/164847733-7edc419c-1021-4565-885d-7362bbf8ebb6.png)
The code (.hex) file is uploaded to the designed circuit in Simulide and working is observed. Among the most important benefits is the elimination of the need of traffic police. The accidents can be reduced by this and Manual labour and stress can be reduced.
