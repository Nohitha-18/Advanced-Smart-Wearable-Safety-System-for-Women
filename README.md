# Advanced-Smart-Wearable-Safety-System-for-Women

## 📌 Overview
This project presents an IoT-based smart wearable safety system designed to enhance women’s safety through automatic emergency detection and real-time communication. Unlike conventional solutions that rely on manual triggering, this system integrates multi-sensor detection to identify potential danger situations and respond automatically.

---

## 🎯 Problem Statement
Most existing safety systems depend on the user pressing a button or manually triggering an alert. In real-world situations such as panic, physical restraint, or unconsciousness, this approach becomes ineffective. There is a need for a system that can automatically detect distress and provide real-time assistance.

---

## 💡 Proposed Solution
The proposed system uses a combination of physiological sensing (heart rate) and interaction detection (touch sensor) to identify potential emergencies. Once detected, it sends continuous alerts including location and image data to predefined contacts via a Telegram chatbot.

---

## ⚙️ System Architecture

### 🔹 Components:
- **Microcontroller:** XIAO ESP32-S3  
- **Sensors:** MAX30105 (PPG), Touch Sensor  
- **Modules:** GPS (NEO-6M), ESP32-CAM  
- **Output Devices:** Vibration Motor, Push Button  
- **Communication:** WiFi + Telegram Bot + Serial Monitor

---

## 🔄 Working Methodology

1. **Continuous Monitoring**
   - Heart rate is monitored using PPG sensor
   - Touch sensor detects external interaction

2. **Data Processing**
   - Raw signals are filtered and converted into meaningful values (BPM)

3. **Decision Logic**
   - If BPM exceeds threshold OR touch is detected → potential emergency

4. **Pre-Alert Stage**
   - Vibration motor alerts user

5. **False Alarm Handling**
   - Push button cancels alert and sends “I am OK” message

6. **Emergency Mode**
   - Image is captured using ESP32-CAM
   - GPS location is fetched

7. **Alert Transmission**
   - Message + image + location sent via Telegram

8. **Continuous Updates**
   - Alerts sent every 20 seconds until stopped

---

## 🔧 Hardware Components
- XIAO ESP32-S3  
- MAX30105 PPG Sensor  
- NEO-6M GPS Module  
- ESP32-CAM  
- Touch Sensor  
- Push Button  
- Vibration Motor  
- Breadboard and Power Supply  

---

## 💻 Software & Tools
- Arduino IDE  
- Embedded C Programming  
- Telegram Bot API  
- WiFi Communication  

---
## 💻 Source Code

The complete implementation of the system is available in the `main.ino` file in this repository.

## 📊 Results
- Successful detection of simulated emergency conditions  
- Real-time alert transmission with location and image  
- Continuous alert mechanism improved reliability  
- False alarm handling reduced unnecessary alerts  

---

## 🚀 Key Features
- Multi-sensor automatic detection  
- Real-time GPS tracking  
- Image-based evidence capture  
- Continuous alert updates  
- False alarm control mechanism  
- Low-cost IoT implementation  

---

## ⚠️ Limitations
- Fixed heart rate threshold (not adaptive)  
- Depends on WiFi connectivity  
- Prototype implemented on breadboard
- GPS not working inside buildings  

---

## 🔮 Future Enhancements
- Adaptive heart rate detection (ML-based)  
- Integration of motion/pressure sensors  
- Mobile application for monitoring  
- GSM/LoRa communication support  
- PCB-based compact wearable design  
- Improved battery efficiency  
- Enhanced GPS accuracy  
- Audio recording for additional evidence  
- Cloud integration for data storage  

---
## Simulation SetUp

---

## 📷 Project Outputs
(Add images here)
- Hardware Setup  
- Telegram Alerts  
- Camera Capture  
- GPS Location Output  

---

## 🧠 Key Learnings
- Embedded systems design  
- IoT communication protocols  
- Sensor integration and processing  
- Real-time system development  

---

## 📌 Conclusion
This project demonstrates a practical IoT-based solution for wearable safety systems by combining automatic detection, real-time communication, and multi-sensor integration, making it more reliable than traditional manual-trigger systems.

---

## 👨‍💻 Authors
- G. Nohitha Navya Sri
## Contributors  
- R. Mohan Suresh  
- G. Satyanandam  

---
## 🧩 My Key Contributions
- Designed hardware architecture  
- Identified limitations in existing systems  
- Led system-level decision logic design  
- Debugged and optimized system performance  
- Assisted in software integration  
---
