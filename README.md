# 🧥 Smart Safety Jacket 

In a world where even able-bodied women face safety concerns, the thought of the challenges encountered by **deaf women** is even more pressing. This conceptual design presents a **wearable safety jacket** aimed at enhancing protection and awareness for deaf women in vulnerable or low-visibility situations. By integrating **sensors, communication modules, and tactile feedback**, the design provides real-time alerts and discreet assistance to the wearer.  
As a part of our *Design Thinking* project I designed a convertible jacket which could also be used as a backpack. 

---

## ✨ Features  

- **GPS Module**  
  - Tracks the wearer’s real-time location.  
  - Can be used to share live coordinates with trusted contacts via cloud services or APIs.  

- **Ultrasonic Sensor**  
  - Continuously monitors surroundings to detect obstacles, approaching entities, or threats.  
  - Calculates distance and movement patterns to warn the wearer.  

- **Vibrational Stimulus**  
  - A vibration motor provides discreet tactile alerts to the wearer.  
  - Alerts can be triggered in two ways:  
    1. Automatically by the system (when a potential threat is detected).  
    2. Manually by the wearer (pressing a button to request feedback or initiate safety mode).  

- **Button-triggered Safety Mode**  
  - When the wearer presses a dedicated button, the jacket:  
    - Sends a signal to trigger vibration feedback.  
    - Sends an emergency notification via Twilio (SMS/Call API) to predefined contacts with the wearer’s location.  

- **Twilio Integration**  
  - Connects the jacket to external communication channels.  
  - Sends **SMS alerts** (including GPS coordinates).  
  - Can be extended to trigger automated phone calls.  

---

## 📐 System Design Overview  

1. **Input Layer**  
   - Ultrasonic sensor → detects distance and movement.  
   - Button press → wearer manually signals distress or requests vibration.  

2. **Processing Layer (ESP32 / Microcontroller)**  
   - Reads data from sensors.  
   - Decides whether to trigger vibration or send an alert.  
   - Connects to WiFi/Bluetooth for cloud/Twilio communication.  

3. **Output Layer**  
   - Vibration motor → tactile feedback.  
   - GPS module → streams location data.  
   - Twilio API → sends emergency notifications to trusted contacts.  

---

## 🛠️ Technologies Considered  

- **Hardware**: ESP32 (for lightweight control + WiFi/BLE), Ultrasonic Sensor (HC-SR04 or equivalent), GPS Module (NEO-6M), Vibration Motor, Push Button, DSSC solar cells (for energy harvesting).  
- **Software**: Arduino IDE / PlatformIO (for prototyping), Twilio API (for communication), optional mobile/web dashboard for tracking.  

---

## 🚀 Potential Applications  

- Safety support for **deaf women in desolate areas at night**.  
- Navigation aid for **visually/hearing-impaired individuals**.  
- Outdoor safety gear for **trekkers, travelers, and workers**.  

---

## 📌 Notes  

⚠️ This project is currently in the **design stage only**. No physical prototype has been developed yet.  
The README serves as **documentation of the concept and design flow**, and may be expanded in the future for implementation.  

---

## 📷 Concept Diagram (Future Addition)  

Images of the design : 
![Image 1] (assets/1.jpg)
![Image 2] (assets/2.jpg)
![Image 3] (assets/3.jpg)
![Image 4] (assets/4.jpg)
---
