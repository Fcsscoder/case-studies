# Estudos de Caso em Sistemas Embarcados e IoT

Esta categoria explora a integração entre hardware microcontrolado, protocolos de mensageria com baixo consumo e aplicações web em tempo real para monitoramento e análise de telemetria ambiental.

---

## Estudos de Caso nesta Trilha

### 1. [Firmware para Telemetria Ambiental e Painel em Tempo Real Orientado a Eventos](real-time-air-quality-iot-telemetry/README.md)
* **Temas Centrais:** Sistemas Embarcados, ESP32, Protocolo MQTT, Arquitetura Orientada a Eventos, Server-Sent Events.
* **Principais Desafios:**
  - Amostrar sensores de gases tóxicos e material particulado a 1 Hz enquanto agrupa e envia pacotes de telemetria via MQTT a cada 30 segundos, poupando energia e rede.
  - Conectar mensagens do broker Mosquitto diretamente ao navegador via Server-Sent Events (SSE), eliminando requisições repetitivas de polling no cliente.
  - Renderizar gráficos temporais contínuos diretamente no elemento HTML5 Canvas com consumo mínimo de memória.
* **Tecnologias:** C++, Arduino/ESP32, Eclipse Mosquitto MQTT, Node.js, Express, EJS, Server-Sent Events, HTML5 Canvas.
