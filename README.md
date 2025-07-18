##### WORK IN PROGRESS . . .

# 📡  APRS_Wx_v1 ( Wemos D1 mini version) Web-Configurable

Configure your ***APRS beacon settings*** entirely through your browser — no hardcoding, no sketch modifications, and absolutely no dependency nightmares. :trollface:

<img src="https://github.com/user-attachments/assets/66c5de3c-2fb3-4ce3-96a6-1faa1181bcd0" alt="prototype" width=28% style="float:left"></p>


---
### <img src="https://user-images.githubusercontent.com/74038190/216122049-276bc7a5-c760-4849-805a-995d8fa6ea13.png" alt="clock" width="6%">  Prototype 

##### (Wx station As "minimalsitic" As Possible)

<img src="https://github.com/user-attachments/assets/a59915d9-7893-41ea-8c82-5707780325c4" alt="prototype" width="400" height="300" style="float:left"></p>

:point_right:  ![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) `Current firmware is under testing by few HAMs , Please contact me if you require the `***bin file***` . `   :point_left:


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

## 🔬 $\color{#fb8a03}{Current~Status!}$
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
<img src="https://github.com/user-attachments/assets/ab9ebb3e-4a45-4d9a-bdc4-5515c6a56e17" alt="pcb1" width="400" height="300" style="float:middle">
      <img src="https://github.com/user-attachments/assets/3069b352-b3dd-4e21-9c63-c1d386fa0aac" alt="pcb2" width="400" height="450" style="float:middle">

> ### $\textcolor{#fc0404}{\textsf{  1st batch of PCB received, Schematic and other details will be updated once PCB testing is done.  }}$
 
<img src="https://github.com/user-attachments/assets/8c59b9ad-8f9f-4441-ab93-16b8d5285eac" alt="pcb3" width=85% style="float:centre"></p>


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

>**Note:** <br>
&#10687; ➡️BMP280 - Temperature Pressure altitude <br>
&#10687; ➡️BME280 - Temperature Pressure altitude humidity <br>
&#10687; Both BMP280 and BME280 modules are available in 4-pin and 6-pin versions. They often look identical and cannot be visually distinguished. <br>
&#10687; To avoid compatibility issues or errors, always purchase from a reliable and reputable seller.

| possible combinations | firmware version | Firmware available |
| :---:  |     :---:        | :---:              |
| DHT11   | 3.1.0 | $\color{#039d05}{&#10003;}$  |	
| DHT11/NTC |	
| DHT11/NTC/OLED  |
| DHT11/OLED 1.3"  |3.1.3 | $\color{#039d05}{&#10003;}$  |	
| DHT11/OLED 0.96"  |3.1.4 | $\color{#039d05}{&#10003;}$  |	
| DHT11 Dual stn   | 3.1.5 | NA  |	
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
| BME280/OLED 1.3"  |	3.5.1 | $\color{#039d05}{&#10003;}$  |	
| BME280/OLED 0.96"  |	3.5.2 | $\color{#039d05}{&#10003;}$  |	
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
https://gist.github.com/rxaviers/7360908  *** emoji
https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

$\color{#FF0000}{Current~Status!}$

#### $\textcolor{blue}{\textsf{Color didint work .}}$

https://github.com/Anmol-Baranwal/Cool-GIFs-For-GitHub?tab=readme-ov-file  *** gif
-->
