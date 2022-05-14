

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

# WORKING 
* The RED LED is considered for the ACC position. Once the push button is pressed for 2 seconds, the RED LED keeps continuously glowing until the stop of the engine signifying the engine condition to be turned ON.
* On press of the user input push button, the other three Blue, Green and Orange LEDs come ON one at a time with the set frequency. The frequency changes on every alternate key press, 3 frequency levels with 1, 4 and 8 Hz.
* The LED glow pattern stops on the 4th press; the wiper action starts with the next press.
* If the push button is pressed for 2 seconds continuously, the RED light goes off and the pattern stops bringing it to default position which signifies the engine is turned OFF.

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
