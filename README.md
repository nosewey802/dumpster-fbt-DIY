# dumpster-fbt-DIY
guide to make the cheapest vr trackers you'll ever see!
An compact, budget friendly DIY full body tracking system for virtual reality (compatible with slimevr), designed to fit all inside of Tic Tac boxes.

# Project Goal
Provide a guide to make full body trackers for the cheapest price to make it more accesible for the people!

# Tracker Setup
* **Main Trackers:** 3 main trackers (ESP32 + IMU + Battery + Enclosure).
* **Extensions:** 3 auxiliary IMUs connected to the main trackers for extra tracking points.

# Hardware & Components

* **Microcontroller:** ESP32-C3 SuperMini
* **Charging Module:** TP4056 with USB-C input.
* **Motion Sensor (IMU):** MPU-6050
* **Battery:** 18650 3.7V rechargeable Li-ion battery
* **Power Switch:** Mini ON/OFF slide switch.
* **Enclosure:** Reused Tic Tac containers 
* **Battery Holder:** Single battery holder.

## Wiring
 ## **MPU6050 and ESP32**
  * VCC --> 3.3V
  * GND --> GND
  * SDA --> GPIO 21
  * SCL --> GPIO 22
 ## **18650 Battery and TP4056**
  * battery (+) --> Pad B+
  * battery (-) --> Pad B-
 ## **TP4056 to power switch to the ESP32**
  * TP4056 (OUT+) --> power switch (center pin)
  * power switch (side pin) --> ESP32 (5V)
  * TP4056 (OUT-) --> ESP32 (GND)

## Software & 3D Modeling

* **Firmware:** SlimeVR firmware loaded onto the ESP32 mini.
* **3D Integration & Modeling:** Component fitment and layout done in Tinkercad.
* **VR Integration:** SteamVR and VRChat tracking integration for torso and limbs.

---

## Repository Structure

```text
dumpster-fbt-DIY/
├── 3D-Models/       # STL models and Tinkercad component fitment screenshots
├── Firmware/        # Pin configuration and flashing instructions
└── README.md        # Project overview and documentation
