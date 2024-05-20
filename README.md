Soldiers Health Monitoring and Position Tracking System
The Soldier Health Monitoring and Position Tracking System allows the military personnel to track the current GPS position of a soldier and also checks the health status including body temperature and heartbeat of a soldier.

Introduction
In this modern era, enemy warfare is one of the most significant factors in any nation’s security. Nation’s security mainly depends on these three specialized uniformed services: The Army, the Air Force, and the Navy. Soldiers are a very essential part of these security systems. During any special operation or mission that’s been carried out by these services, soldiers involved tends to get injured or get lost on the battlefield. As the soldier plays a significant role in national security, we cannot afford to let them get lost, or have any delayed medics reach the injured ones. So, to protect these soldiers we should have some technology that monitors and tracks the soldiers in real-time and help minimize the time of search operation, and rescue operation efforts of the control unit.

So, to support this idea, the project presents an effectual system that is capable of monitoring the health vitals of soldiers and at the same time able to record their current position using necessary sensors. The data collected from the sensors are then transmitted to the next level of the hierarchy using wireless RF modules. This system enables the control room unit to track the location and monitor the health vitals of the soldiers constantly using the wireless body sensor network, and the GPS receiver at frequent intervals. Arduino associated with the control room constantly monitors the data received from the different subsystems of the proposed design and triggers a warning if any values cross the set threshold values. Live health monitoring and position tracking of the soldiers will ensure that they are safe on the battlefield and if any abnormalities are found in the values received to the control unit node, they make sure that relief is sent from the control unit node or the squadron leader’s node within a minimum amount of time.

This system in particular will be useful for individuals, who involve in missions or in special operations.
Extra libraries
The extranal librarires used in the project.

TinyGPS++ : https://github.com/mikalhart/TinyGPSPlus
PulseSensorPlayground : https://github.com/WorldFamousElectronics/PulseSensorPlayground
LoRa: https://www.arduino.cc/reference/en/libraries/lora/
Clone the repos and add the folder to the libraries folder in Arduino IDE.
METHODOLOGY
Components Required
Arduino UNO (x3)
Temperature Sensor - LM35 (x2)
Pulse Sensor - RC-A-4015 (x2)
GPS Receiver - Neo-6M (x2)
HC-12 RF module
SX-1278 RF LoRa module
9V 3A Battery
Breadboard and jumper wires
Components Descriptions
HC-12 Sensor
HC-12 wireless serial port communication module is a new-generation multichannel embedded wireless data transmission module. The HC-12 is a half-duplex 20 dBm (100 mW) transmitter paired with a receiver that has -117 dBm (2×10-15 W) sensitivity at 5000 bps. Paired with an external antenna, these transceivers are capable of communicating up to and possibly slightly beyond 1 km in the open and are more than adequate for providing coverage throughout a typical house. Its wireless working frequency band is 433.4-473.0MHz, multiple channels can be set, with the stepping of 400 KHz, and there are totally 100 channels.

SX-1278
The SX1278 transceiver feature the LoRa long range modem that provides ultra-long range spread spectrum communication and high interference immunity whilst minimizing current consumption. Using Semtech’s patented LoRa modulation technique SX1278 can achieve a sensitivity of over -148dBm using a low cost crystal and bill of materials. The high sensitivity combined with the integrated +20dBm power amplifier yields industry leading link budget making it optimal for any application requiring range or robustness. LoRa also provides significant advantages in both blocking and selectivity over conventional modulation techniques, solving the traditional design compromise between range, interference immunity and energy consumption.

WORKING
The system has two sections, hardware and software. The system consists of 3 nodes i.e Soldier’s node, Squadron leader’s node, and Control unit node. At all the nodes Arduino constantly monitors and records data from the several sensors connected to the system, and communicates with other nodes using wireless RF modules present in the system.

The hierarchy of obtaining data from the soldier is divided into three segments:
Soldier's Node - Level 1
Squadron's Node - Level 2
Control unit Node - Level 3
