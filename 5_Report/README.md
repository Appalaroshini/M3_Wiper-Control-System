
## Abstract

For this project, we use the STM32F4xx-discovery board to display the vehicle filter control system. Most car wires are controlled by a DC motor, however because the STM32F4xx-discovery does not have an engine, we test using LEDs in this application. For example, wiper control system. The STM32F4xx-discovery board has four LEDs and a Push Button. The colors of these LEDs are orange, green, red and blue. Current limit resistance connects four user LEDs to PD12, PD13, PD14, and PD15 PORTD pins on the Recovery board. To activate the push button with the STM32F407VG controller, GPIO PINs will be set as digital input pins. When you press and hold the user button for two seconds, Red When the ignition key is set to ACC, the LED turns on. In addition, the LEDs flash, indicating that the wipers are on.

The operation of the windshield wiper is a manual operation that requires opening to remove rain and debris from the screen. This not only requires the driver's attention, but also, causes a certain degree of discomfort to the driver and serves as a source of distraction that increases the risk of accidents. To comfort the driver and reduce the risk of accidents, an automatic rain sensor is now a must. Although such a device is available on the market, its high cost and other similar limitations have made it relatively popular in the automotive industry. The aim of this project was to promote another cost-effective model in the market while maintaining efficiency. Rain sensor, microcontroller and integrated driver circuit (IC) are the major components used in the construction and operation of the proposed device. Falling water is quickly and accurately detected by a rain sensor and transmits the signal to the second component i.e..microcontroller which gives the driver IC the ability to change the required movement of the wires when using a servo motor. This device converts hard manual labor into smooth automatic.




# REQUIREMENTS 
## STM32Cube IDE 
* STM32Cube software ecosystem. STM32CubeIDE is an advanced C/C++ development platform with peripheral configuration, code generation, code compilation, and debug features for STM32 microcontrollers and microprocessors. It is based on the Eclipse®/CDT™ framework and GCC toolchain for the development, and GDB for the debugging. It allows the integration of the hundreds of existing plugins that complete the features of the Eclipse® IDE.


## Xpack Packages 

 Windows Build Tools

 OpenOCD 

 QEMU 

## COMPONENTS

### STM32F407G-DISC1

STM32F407 series of microcontrollers are high-performance MCUs designed for medical, industrial and consumer applications. It is based on ARM Cortex-M4 and offers up to 168MHz. The STM32F407VGT6 is the onboard chip which comes in a 100-pin LQFP package.

The STM32F407G-DISC1 is a Discovery Kit allows users to easily develop applications with the STM32F407 high performance microcontrollers with ARM cortex-M4 32-bit core. It includes everything required either for beginners or for experienced users to get quickly started. Based on the STM32F407VGT6, it includes an ST-LINK/V2 or ST-LINK/V2-A embedded debug tool, two ST MEMS digital accelerometers, a digital microphone, one audio DAC with integrated class D speaker driver, LEDs and push buttons and an USB OTG micro-AB connector.

### Features Of STM32F407G
* Flash memory of up to 1 megabyte.
* OTP memory of 512 bytes.
* Compact Flash, SRAM, PSRAM, NOR, and NAND memories are supported by this flexible static memory controller.
* Sleep, Stop, and Standby modes are low-power modes.
* 16-stream DMA controller with FIFOs and burst support for general-purpose DMA.
* Up to 54 Mbytes/s 8- to 14-bit parallel camera interface.
* Generator of true random numbers.
* Hardware calendar, CRC calculating unit, 96-bit unique ID RTC, subsecond accuracy.


 ## 4 W'S
#### WHAT IS WIPER SYSTEM
  * Windscreen wipers are necessary for maintaining sufficient view for the driver, especially in modern high-speed cars.
#### WHY WIPER SYSTEM
  * To keep the windscreen clean enough to give adequate view at all times.
#### WHEN SHOULD USE WIPER SYSTEM 
  * The windshield wipers remove rain and snow from the windshield, while the headlights improve visibility at night.
#### WHO DISCOVERED WIPER SYSTEM
 * Mark Anderson invented on 1902

# SWOT ANALYSIS
### Strengths
a) Growth in production of vehicles

b) Higher demand for luxury features

c) Automatic wiper control system

d) Less power consumption

e) Operating level is easy

### Weakness
a) May not be working at inclement weather

b) May not detect objects

c) It may also malfunction if components fail

d) Sometimes not working properly

e) High cost

### Opportunities
a) The wiper serves to clean the windshield of the any automobile at the front and rear. Wiper works by removing oil, dust, rainwater, and dirt that get stuck to the windshield.

b) Wipers detect moisture on the windshield and activate the wipers to help increase driver visibility.

c) Improve safety by decressing driver distraction.

### Threats
a) Time interval may vary thereby it cause some problem on wiper system.

b) Due to so much ice or snow on windshield may cause the wipers to get jammed and cause circuit overloading.

c) Accident may occur due to fault in wiper system.




### High Level Requirements
| RID | Description | Status |
| -- | ----------- | ------ |
| HLR1 | EMBEDDED C LANGUAGE | IMPLEMENTED |
| HLR2 | OS WINDOWS | IMPLEMENTED |
| HLR3 | STM32CUBEIDE | IMPLEMENTED |
| HLR4 | CYGWIN | IMPLEMENTED |
| HLR5 | QEMU  | IMPLEMENTED |
| HLR6 | HARDDISK | IMPLEMENTED |
| HLR7 | RAM 4GB | IMPLEMENTED |


### Low Level Requirements
| RID | Description | Status |
| -- | ----------- | ------ |
| LLR1 | RED LED ON | IMPLEMENTED |
| LLR2 | BLUE LED FREQUENCY 1HZ | IMPLEMENTED |
| LLR3 | GREEN LED FREQUENCY 4HZ | IMPLEMENTED |
| LLR4 | ORANGE LED FREQUENCY 8HZ | IMPLEMENTED |
| LLR5 | RED LED OFF  | IMPLEMENTED |

## Design
## Flow chart 

![image](https://user-images.githubusercontent.com/101495481/168426038-20ca0e70-2797-4150-b7e7-96753cd00b34.png)



## Schematic diagram 

![image](https://user-images.githubusercontent.com/101495481/168426073-0ae72b6f-4970-4fc0-bc6b-f5b790941a5c.png)


Block Diagram:

![image](https://user-images.githubusercontent.com/101495481/168425936-7726046f-e14c-4a3f-b2a1-d1d181a92170.png)

# Output

![image](https://user-images.githubusercontent.com/101495481/168429100-cc49fa19-7e9a-4163-b0f5-825a45493efc.png)
![image](https://user-images.githubusercontent.com/101495481/168429109-e7fd934b-108a-44f1-9821-9cf2144d09ab.png)
![image](https://user-images.githubusercontent.com/101495481/168429124-08402b75-4ba5-4f70-93ee-98aa180ab5ba.png)
