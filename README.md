
---

# 🐟 **AQUA – Smart Fish Monitoring System**

**Live Demo:** [https://aquafish-pi.vercel.app/](https://aquafish-pi.vercel.app/)

AQUA is a smart IoT-enabled fish farming monitoring system that uses sensors, automation, and real-time data analytics to help fish farmers track pond conditions, reduce fish mortality, and improve productivity.
The system integrates **MongoDB**, **Firebase Realtime Database**, and **ESP32 microcontrollers** for a complete end-to-end solution.

---

## 🚀 **Key Features**

### **🌡️ Real-Time Water Monitoring**

* Temperature
* pH level
* Dissolved Oxygen (DO)
* Turbidity
* Ammonia levels
* Water depth/level

### **⚙️ Smart Automation**

* Automatic fish feeder
* Aerator auto-activation when oxygen is low
* Pump control when water level is low/high
* Auto adjustment based on sensor thresholds

### **📡 Real-Time Database Sync**

* Live sensor values saved in **Firebase Realtime Database**
* Historical data stored in **MongoDB**
* Dashboard updates instantly without refresh

### **📲 Web Interface Dashboard**

Visit the live dashboard:
👉 **[https://aquafish-pi.vercel.app/](https://aquafish-pi.vercel.app/)**

Features:

* Real-time charts
* Device control (aerator, feeder, pump)
* Alerts log
* Daily/weekly trends
* Monitoring multiple ponds

### **🔔 Notifications**

* Threshold alerts (SMS/Email/Push)
* Water quality warnings
* Feeding reminders

---

## 🛠️ **Tech Stack**

### **Hardware**

* ESP32
* DS18B20 Temperature Sensor
* pH Sensor
* Turbidity Sensor
* DO Sensor
* Ultrasonic sensor (water level)
* Relay modules
* Auto Feeder system
* Aeration Motor

### **Software**

| Component               | Technology                 |
| ----------------------- | -------------------------- |
| Frontend                | React + Tailwind           |
| Backend                 | Node.js / Express          |
| Database 1 (Realtime)   | Firebase Realtime Database |
| Database 2 (Historical) | MongoDB                    |
| Hosting                 | Vercel / Render            |
| Communication           | Firebase SDK + REST APIs   |
| Microcontroller         | Arduino IDE (ESP32)        |

---

## 📦 **Installation & Setup**

### **1. Clone the repository**

```bash
git clone https://github.com/your-username/aqua-smart-monitoring.git
cd aqua-smart-monitoring
```

### **2. Install backend dependencies**

```bash
npm install
```

### **3. Environment variables**

Create a `.env` file:

```
MONGO_URI=your_mongodb_connection_string
FIREBASE_API_KEY=your_firebase_key
FIREBASE_DB_URL=your_realtime_db_url
JWT_SECRET=your_secret
FEEDER_PIN=13
AERATOR_PIN=12
PUMP_PIN=14
```

### **4. Run backend**

```bash
npm run dev
```

### **5. Setup ESP32**

Configure the following in your ESP32 code:

* WiFi SSID & password
* Firebase RTDB credentials
* Backend API URL
* Sensor pins

Upload using Arduino IDE or PlatformIO.

---

## 🧪 **Core Functionalities**

| Feature                   | Description                                  |
| ------------------------- | -------------------------------------------- |
| Live Sensor Streaming     | Firebase updates every 1–5 seconds           |
| Historical Logging        | Saved in MongoDB                             |
| AI Suggestions (optional) | Predict fish growth or feeding needs         |
| Device Control            | Feeder, aerator, pump                        |
| Alerts                    | Based on unsafe water parameters             |
| Multi-Pond Support        | Manage multiple fishponds from one dashboard |

---

## 📊 **Dashboard Features**

Visit: **[https://aquafish-pi.vercel.app/](https://aquafish-pi.vercel.app/)**

Includes:

* Live water quality charts
* Water Quality Index (WQI) calculations
* Fish health recommendations
* History graphs
* Device toggle controls
* Real-time alerts

---

## 📈 **Future Enhancements**

* Machine learning to predict disease outbreaks
* Camera-based fish counting
* Solar-powered microcontroller setup
* Offline mode with local caching
* Voice assistant control
* SMS/WhatsApp integration for alerts

---

## 🤝 **Contributing**

1. Fork the repo
2. Create a feature branch
3. Commit and push
4. Submit a pull request

---

## 👨‍💻 Developer

**Willington Juma**
Software Developer • IoT Enthusiast • Data Engineer

---

## 📜 License

MIT License – free to use and modify.

---


