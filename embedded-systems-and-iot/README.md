# Embedded Systems & IoT Case Studies

This category covers embedded firmware development, low-power sensor sampling, publish/subscribe messaging protocols, and event-driven web dashboard integration.

---

## Case Studies in this Track

### 1. [Real-Time Environmental Telemetry Firmware & Event-Driven Dashboard](real-time-air-quality-iot-telemetry/README.md)
* **Core Themes:** Embedded C++, ESP32 Microcontrollers, MQTT Pub/Sub, Server-Sent Events (SSE), Real-Time Canvas Graphing.
* **Key Challenges:**
  - Decoupling continuous 1 Hz analog sensor reads (MQ135 volatile gases and PM2.5 optical dust sensors) from batched 30-second MQTT telemetry transmissions to optimize power and network bandwidth.
  - Streaming live telemetry from an Eclipse Mosquitto broker directly to a browser client over Server-Sent Events (SSE), eliminating client-side HTTP polling.
  - Rendering lightweight time-series charts directly onto an HTML5 Canvas buffer without third-party library memory overhead.
* **Technologies:** C++, Arduino/ESP32, Eclipse Mosquitto MQTT, Node.js, Express, EJS, Server-Sent Events, HTML5 Canvas.
