# 📡  APRS_Wx_v1 ( Wemos D1 mini version) Web-Configurable

Configure your ***APRS beacon settings*** entirely through your browser — no hardcoding, no sketch modifications, and absolutely no dependency nightmares. :trollface:

<img src="https://github.com/user-attachments/assets/092c29cf-3f0c-4288-83ee-a94c555be458" alt="prototype" width=25% style="float:left"></p>

---
### Prototype
##### (Wx station As "minimalsitic" As Possible)

<img src="https://github.com/user-attachments/assets/a59915d9-7893-41ea-8c82-5707780325c4" alt="prototype" width="400" height="300" style="float:left"></p>

---

## ✨ Features
- 🔧 **Fully browser-configurable**: APRS callsign, GPS Coordinates, interval, WiFi, and more.
- 💾 **Persistent storage**: Settings are saved to flash and survive reboots.
- 🔁 **Live configuration**: Changes take effect without reflashing firmware.
- 📱 **Mobile-friendly interface**: Configure from your phone, tablet, or laptop.
- 🔒 **Secure WiFi setup**: AP + STA mode for easy setup and permanent operation.
- 🌍 **OTA update support** *(optional)*: Upload new firmware from the browser. (future implementation) 
---

## 📦 Hardware Requirements
- ✅ **Wemos D1 Mini** – ESP8266-based microcontroller
- ✅ Sensors based on your selected `firmware`
- ✅ Power source (USB 5V or 5-6v adaptor)
- ✅ Optional: OLED display
---

## 🔌 Wiring Diagram 🌐 Usage Guide
- Depends on your sensor / Check PDF.
---

## 🔁 Resetting Configuration
To reset all settings:
- Put device in **Config mode** & make the required changes.
---

## 🔧 Dependencies
- ESPAsyncWebServer
- EEPROM
- WiFiManager *(or custom captive portal implementation)*
- APRS packet formatting utilities
- Many more . . .

These are **pre-integrated** in the firmware. You do **not** need to manage library versions manually . :smiley:

---

## 🛠️ Roadmap
- [ ]  Display Sensor data on OLED screen
- [ ] GPS-based dynamic beaconing (position changes in real time)
- [ ] Password protection for the config web page
- [ ] OTA firmware upload via web interface
- [ ] Support for digipeater functionality
- [ ] Automatic time synchronization via NTP
- [ ] Display Sensor data on the web page
- [ ] Advanced beacon scheduling (time-of-day, speed-based, etc.)
---

## 🔬 $\color{#0321fb}{Current~Status!}$
- ✅ **Beta testing in progress** with HAM operators.
 
- 📦 **Current firmware version includes:**
   - 🌡️ Support for **DHT11**
   - 🌡️ Support for **BME280**
- 🧪 These sensor-enabled builds are undergoing real-world testing for:
   - performance in real-world APRS conditions.
   - Browser-based configuration reliability.

> ## All Instructions to build and test the prototype has been given in the pdf.
 
nodemcu-flasher download <a href="https://drive.google.com/drive/folders/1Jr-8lz06fxJDTsEEtfGwZtn3OogKy-7V?usp=sharing">link</a>


### sample PCB
<img src="https://github.com/user-attachments/assets/ab9ebb3e-4a45-4d9a-bdc4-5515c6a56e17" alt="pcb" width="400" height="300" style="float:middle">
      <img src="https://github.com/user-attachments/assets/3069b352-b3dd-4e21-9c63-c1d386fa0aac" alt="pcb" width="400" height="300" style="float:middle">

> ### $\textcolor{#fc0404}{\textsf{  PCB is under fabrication ! }}$


| Supported Senors |
| :---: | 
| DHT11 | 
| DHT22 |
| RAIN   |
| BMP180  |
| BMP280  |
| BME280  |
| OLED Display  |
| GPS  |
| NTC  |
| LDR  |

| possible combinations | firmware version | Firmware available |
| :---:  |     :---:        | :---:              |
| DHT11   | 3.1.0 | $\color{#039d05}{&#10003;}$  |	
| DHT11/NTC |	
| DHT11/NTC/OLED  |
| DHT22  |		
| DHT22/NTC |	
| DHT22/OLED  |	
| BMP180  | 		
| DHT11/BMP180  |	
| DHT11/BMP180/OLED  |
| BMP280  | 		
| DHT11/BMP280  |	
| DHT11/BMP280	OLED  |
| BME280  | 	 3.5.0 | $\color{#039d05}{&#10003;}$  |	
| BME280/OLED  |	
| DHT11/GPS |	
| DHT11/GPS/OLED  |
| DHT22/GPS/OLED  |
| DHT11/LDR |	
| DHT11/OLED/LDR  |
| DHT22/LDR  |	
| DHT22/OLED/LDR  |






 > ##### My Iteration Versions:
 > - Nodemcu - v1
 > - esp8266-01 - v2
 > - Wemos D1 Mini - v3





<!-- 
 [ ] for pending items and [x] for completed ones.
-->

<!-- 
## 🧰 Development / Custom Builds

Want to build your own version?

```bash
# Clone the project
git clone https://github.com/yourusername/APRS-WebConfig-D1Mini.git
cd APRS-WebConfig-D1Mini

# Open in Arduino IDE or PlatformIO
# Modify src/main.cpp as needed
---
-->

<!--

cheat sheet
https://gist.github.com/rxaviers/7360908

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

$\color{#FF0000}{Current~Status!}$

#### $\textcolor{blue}{\textsf{Color didint work .}}$
-->
