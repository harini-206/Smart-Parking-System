# Smart-Parking-System
 This Smart Parking System uses an ESP32 microcontroller and ultrasonic sensors to monitor the availability of parking slots in real time.The system helps drivers quickly identify free parking spaces, reducing time, fuel consumption, and traffic congestion. It provides an automated, efficient, and IoT-based parking management solution.
 
# Blynk 
Blynk is an IoT cloud platform that allows us to connect hardware devices like ESP32 to a mobile or web application for real-time monitoring and control.

in our Smart Parking System, Blynk helps by displaying live parking information such as the distance measured by the ultrasonic sensor, slot occupancy status, number of occupied slots, and available slots. The ESP32 sends sensor data to the Blynk cloud using Wi-Fi, and the Blynk app shows this data through user-friendly widgets like gauges, LEDs, and labels. This makes the system easy to monitor remotely, improves efficiency, and provides a clear visual representation of parking availability in real time.


# Steps to Integrate IoT Device with Blynk

Create an account and log in to the Blynk Cloud platform.

Create a new template by selecting the hardware as ESP32 and the connection type as Wi-Fi.

Add required datastreams using virtual pins to send sensor data to the Blynk application.

Create a device from the template and obtain the unique authentication token.

Include Blynk libraries in the ESP32 program and add the template ID, authentication token, and Wi-Fi credentials.

Design the dashboard in the Blynk app by adding widgets such as gauge, LED, and value display, and link them to the virtual pins.

Program the ESP32 to read sensor data and send it to Blynk using virtual pin communication.

some screenshots of how it  created  it :

<img width="894" height="596" alt="image" src="https://github.com/user-attachments/assets/29f46deb-ae25-414a-bfcd-1b2d8790f19a" />


<img width="1016" height="476" alt="image" src="https://github.com/user-attachments/assets/80e52a9a-a5eb-47c6-8341-092fd6096838" />

<img width="1295" height="628" alt="image" src="https://github.com/user-attachments/assets/3f74b85a-a225-4c35-b120-ff159ecd892a" />



| Widget | Virtual Pin | Input Type | Purpose               |
| ------ | ----------- | ---------- | --------------------- |
| Gauge  | V0          | Integer    | Displays distance     |
| LED    | V1          | Integer    | Slot occupancy status |
| Label  | V2          | Integer    | Occupied slots        |
| Label  | V3          | Integer    | Available slots       |





Upload the code to the ESP32, connect it to the internet, and monitor real-time data through the Blynk application.

