
## Abstract

For this project, we use the STM32F4xx-discovery board to display the vehicle filter control system. Most car wires are controlled by a DC motor, however because the STM32F4xx-discovery does not have an engine, we test using LEDs in this application. For example, wiper control system. The STM32F4xx-discovery board has four LEDs and a Push Button. The colors of these LEDs are orange, green, red and blue. Current limit resistance connects four user LEDs to PD12, PD13, PD14, and PD15 PORTD pins on the Recovery board. To activate the push button with the STM32F407VG controller, GPIO PINs will be set as digital input pins. When you press and hold the user button for two seconds, Red When the ignition key is set to ACC, the LED turns on. In addition, the LEDs flash, indicating that the wipers are on.

The operation of the windshield wiper is a manual operation that requires opening to remove rain and debris from the screen. This not only requires the driver's attention, but also, causes a certain degree of discomfort to the driver and serves as a source of distraction that increases the risk of accidents. To comfort the driver and reduce the risk of accidents, an automatic rain sensor is now a must. Although such a device is available on the market, its high cost and other similar limitations have made it relatively popular in the automotive industry. The aim of this project was to promote another cost-effective model in the market while maintaining efficiency. Rain sensor, microcontroller and integrated driver circuit (IC) are the major components used in the construction and operation of the proposed device. Falling water is quickly and accurately detected by a rain sensor and transmits the signal to the second component i.e..microcontroller which gives the driver IC the ability to change the required movement of the wires when using a servo motor. This device converts hard manual labor into smooth automatic.



# WORKING 
* The RED LED is considered for the ACC position. Once the push button is pressed for 2 seconds, the RED LED keeps continuously glowing until the stop of the engine signifying the engine condition to be turned ON.
* On press of the user input push button, the other three Blue, Green and Orange LEDs come ON one at a time with the set frequency. The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz.
* The LED glow pattern stops on the 4th press; the wiper action starts with the next press.
* If the push button is pressed for 2 seconds continuously, the RED light goes off and the pattern stops bringing it to default position which signifies the engine is turned OFF.

# REQUIREMENTS 
## STM32Cube IDE 
* STM32Cube software ecosystem. STM32CubeIDE is an advanced C/C++ development platform with peripheral configuration, code generation, code compilation, and debug features for STM32 microcontrollers and microprocessors. It is based on the Eclipse®/CDT™ framework and GCC toolchain for the development, and GDB for the debugging. It allows the integration of the hundreds of existing plugins that complete the features of the Eclipse® IDE.


## Xpack Packages 

### Windows Build Tools
* The xPack Windows Build Tools is a standalone Windows binary distribution of GNU make and a few of other tools required by the Eclipse Embedded CDT (formerly GNU MCU/ARM Eclipse) project, but the binaries can also be used in generic build environments.

### OpenOCD 
* Open On-Chip Debugger (OpenOCD) is a free, open-source project that aims to provide debugging, in-system programming, and boundary scan using a debug adapter. The adapter is a hardware module that provides the right signals for the target to understand.

### QEMU 
* The xPack QEMU Arm is a standalone cross-platform binary distribution of QEMU, with several extensions for Arm Cortex-M devices.

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


# REQUIREMENTS
## High level requirements
| ID | Description | Status |
| --- | --- | --- | 
| HR_01 | ACC Mode Operation |	Implemented |
| HR_02 |	Wiper ON |	Implemented |
| HR_03 |	Wiper Speed Change |	Implemented |
| HR_04 |	Wiper OFF |	Implemented |
## Low level requirements
| ID |	Description | Operation |	Status |
| --- | --- | --- | --- |
| LR_01 |	Button pressed once for 2 secs | Red LED ON |	Implemented |
| LR_02 |	Button pressed second time | 1 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_03	|Button pressed third time | 4 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_04	|Button pressed fourth time | 8 Hz speed - Blue, Green Orange alternative |	Implemented |
| LR_05 |	Button pressed again for two seconds |Turn Off all LEDs |	Implemented |

## Design
## Flow chart 

![image](https://user-images.githubusercontent.com/101495481/168426038-20ca0e70-2797-4150-b7e7-96753cd00b34.png)



## Schematic diagram 

![image](https://user-images.githubusercontent.com/101495481/168426073-0ae72b6f-4970-4fc0-bc6b-f5b790941a5c.png)


Block Diagram:

![image](https://user-images.githubusercontent.com/101495481/168425936-7726046f-e14c-4a3f-b2a1-d1d181a92170.png)

# Output

