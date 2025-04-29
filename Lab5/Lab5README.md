# Lab 5 - MQTT Communication using Mosquitto and Python

## Objective
This lab demonstrates how to implement MQTT communication using the Mosquitto broker and Python's Paho-MQTT library. Both basic publish/subscribe functionality and CPU usage data transmission were tested.

---

## Screenshot 1  
**Paho-MQTT library successfully installed using pip on Windows.**  
This is required for all Python-based MQTT scripts.
![lab5#1](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%231.png?raw=true)

---

## Screenshot 2  
**Testing message publishing and subscription using Mosquitto in MinGW64.**  
The left terminal publishes a message, and the right terminal receives it.
![lab5#2](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%232.png?raw=true)

---

## Screenshot 3  
**Paho-MQTT successfully installed inside the MinGW64 environment.**  
This allows Python MQTT scripts to run from MinGW64 instead of Command Prompt.
![lab5#3](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%233.png?raw=true)

---

## Screenshot 4  
**Kevinwlu’s IoT repository cloned from GitHub.**  
This repo contains the lab scripts, including pub.py, sub.py, and pubcpu.py.
![lab5#4](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%234.png?raw=true)

---

## Screenshot 5  
**client.py script listening to Mosquitto system topics.**  
It prints broker statistics like number of messages sent, received, or dropped.
![lab5#5](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%235.png?raw=true)

---

## Screenshot 6  
**Testing pub.py and sub.py Python scripts in MinGW64.**  
A “Hello” message is published and received over the topic `paho/test`.
![lab5#6](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%236.png?raw=true)

---

## Screenshot 7  
**Running pub-multiple.py and sub-multiple.py on multiple MQTT topics.**  
This verifies message handling on multiple channels in parallel.
![lab5#7](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%237.png?raw=true)

---

## Screenshot 8  
**Publishing live CPU usage data using pubcpu.py and subcpu.py in Command Prompt.**  
The subscriber prints timestamped CPU percentages received from the publisher.
![lab5#8](https://github.com/acana68/Engineering-Design-VI/blob/main/Lab5/lab5%238.png?raw=true)

---

## Summary
This lab confirmed successful installation and execution of MQTT broker/client communication through both MinGW64 and native Windows terminals. MQTT messages were exchanged over single and multiple topics, and system stats were streamed using Python scripts.

