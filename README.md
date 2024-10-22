# Military Purpose Robot Using Arduino Uno R3

### Introduction :
The project is design to Military Purpose Robot using some different type of sensors for its movement. Arduino uno and different ICs used to achieve the desired operation. Monitoring a group of circumstances, a region, or a person is the task of surveillance. This typically happens in a military setting where monitoring enemy territory, hostage situations, or conflict zones is essential to a country's security. A surveillance robot is a semi automated machine that follows instructions, gathers necessary data, strives to reach its target, and streams or captures photos that can be examined by the operator while avoiding obstacles. Our goal in this Project is to offer a solution or example for a wirelessly controlled robot vehicle that can recognise an object, gauge how far away a human is from the vehicle, and wirelessly feed video of its surroundings to the operatored and detects landmines using a metal detector coil. Once detected the vehicle transmits the GPS location of the landmine over an SMS to the registered phone number so that the mine locations can be mapped.

### Block Diagram :
1) GPS module system
<img width="482" alt="Screenshot 2024-10-22 164625" src="https://github.com/user-attachments/assets/437af900-ad9c-47b9-8c5e-10f08a673711">

   
2) Surveillance robot using ESP32 cam module
<img width="232" alt="Screenshot 2024-10-22 164632" src="https://github.com/user-attachments/assets/bcdec5c0-dba5-4ebf-a7ee-f0fe22c6f8e5">

### Hardware : 
1. ESP32 cam module 
2. L298N Motor Driver 
3. Global Positioning System (GPS) Module 
4. Metal Sensor  
5. LCD Display 16*2 
6. Power  
7. Connecting wires


### Software :

1. Arduino IDE

### Pin Connection :
1) Connect L298 Motor Driver to DC motor:

<img width="469" alt="Screenshot 2024-10-22 165039" src="https://github.com/user-attachments/assets/f9c833f5-e29e-4082-a16f-8370edcd688d">

Notes: We will connect the motors in criss cross pattern. This is because we have to make the car in such a way that two side motor rotates in same direction in order to go Forward Backward and other known directions

2) Connect L298 Motor Driver to ESP32 Cam module:

<img width="460" alt="Screenshot 2024-10-22 165157" src="https://github.com/user-attachments/assets/c604f8b9-2f55-4a73-8df9-cff3927c64ba">


3) Connect ESP32 Cam Module to Arduino UNO:

<img width="465" alt="Screenshot 2024-10-22 165230" src="https://github.com/user-attachments/assets/790f92fd-ee1c-4a8a-8a2f-db1e7c514589">

4) Connect GPS Module to Arduino UNO:
<img width="469" alt="Screenshot 2024-10-22 165342" src="https://github.com/user-attachments/assets/9b81a701-9dbe-4ad5-9e4f-0af9f539fe86">

5) Connect LCD 16*2 to Arduino UNO: 
I. Control pin RS, RW and En are directly connected to Arduino uno pin 12, GND and 11 respectively
II. Data pin D4 to D7 is connected to pins 5, 4, 3 and 2 respectively of Arduino uno

6) Connect DHT11 to ESP32 Cam module: 
<img width="467" alt="Screenshot 2024-10-22 165517" src="https://github.com/user-attachments/assets/1d901c6d-ccd6-4c11-9c74-a38d7f393bf5">

### Working :
1)  Landmine detection and GPS module system \
The robotic vehicle consists of Node MCU (ESP8266) connected with four wheels for the movement of the vehicle over the land in clockwise and anti-clockwise direction. In front side of robotic vehicle metal detector is placed which can sense mine ahead of it. When a Landmine is detected the robotic vehicle halts at that position and activates the GPS module. The GPS data is extracted online to get the latitude and longitude information of a particular location and transfer it to the blynk app at the controlling end. The ESP8266 Wi-Fi Module is a selfcontained SOC with combined TCP/IP protocol stack that can give access to your Wi-Fi network. The ESP8266 is proficient of either introducing an application or offloading all Wi-Fi networking functions from other application. Which gets the latitude and longitude location through online access and give it to the blynk app. The system consists of two main modules, which are control station which runs on a PC or mobile and remotely controlled robot. The control station consists of three integrated modules consisting of Metal detecting component, GPS data collecting component and Remote-control component. These three components act as one system but the original system components act as instantaneously working autonomous systems.

2) Surveillance robot using ESP32 cam module \
This robot has basically three module the first one is ESP32-cam module the second one motor driver module and the third one TP5100 which can be used as power supply and charge management module. This project aims are designing a robot which can be controlled wirelessly via Wi-Fi module with help of our smartphone and PC. This robot has five controlled (go, back, left, right, stop) and capable of moving in all four directions. The main advantages of this project are economically low. This wireless controlled robot can be used for different sophisticated robotic applications. This wireless robot can be controlled by Node MCU ESP32-cam microcontroller. The data sent by our smartphone and PC can be received over Wi-Fi module which is connected to our microcontroller.

![Military Purpose Robot 7](https://github.com/user-attachments/assets/9156c408-8fb7-4472-8f14-2c9cf3e31f14)

![Military Purpose Robot 8](https://github.com/user-attachments/assets/84ea974a-f112-441a-967f-5be87ed4cbc3)

![Military Purpose Robot 9](https://github.com/user-attachments/assets/dd111d31-8109-491b-bd1b-c92d0cb6efc9)

![Military Purpose Robot 6](https://github.com/user-attachments/assets/5125561b-1722-4bd6-804a-24deb17abc0a)

![Military Purpose Robot 4](https://github.com/user-attachments/assets/cc54c1a5-fd48-4b53-b594-6e6e74990764)

![Military Purpose Robot 3](https://github.com/user-attachments/assets/df83cc12-60a0-4f7d-90b0-f3cb4f4ba293)

![Military Purpose Robot  11](https://github.com/user-attachments/assets/d770bddc-e737-4b88-a75e-302ce949da0b)
