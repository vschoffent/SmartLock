🔒 SmartLock - Sistema de Fechadura Inteligente com ESP32 e MQTT
Um sistema IoT que permite o controle remoto de uma fechadura via ESP32, utilizando comunicação MQTT, um servidor Node.js e um aplicativo web em JavaScript.

Diagrama do Sistema

<img src="https://private-user-images.githubusercontent.com/69463307/330925299-235c43b4-aefd-460a-ad91-8b96f89ced99.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDg0NzM3MjYsIm5iZiI6MTc0ODQ3MzQyNiwicGF0aCI6Ii82OTQ2MzMwNy8zMzA5MjUyOTktMjM1YzQzYjQtYWVmZC00NjBhLWFkOTEtOGI5NmY4OWNlZDk5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA1MjglMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNTI4VDIzMDM0NlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTZkZDkyMTlhZTdmYWY0MzMyZDQ3OTA3N2JlNGNiNDE0ODM3NDMyZjJjNGVhZWEzOGI4Y2FiMGE0ZWYxNTJkNWYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.yHXe_5yKHvgzasO1uRgRcBVvbadhRpwvB5O415W5oGc" width=50%/>


🛠 Tecnologias Utilizadas
- Hardware: ESP32 (com Wi-Fi e Bluetooth).
- Protocolo: MQTT (broker: [Mosquitto/CloudMQTT/HiveMQ]).
- Backend: Node.js (com bibliotecas mqtt, express).
- Frontend: JavaScript (Vanilla JS ou framework como React/Vue).
- Firmware: Arduino/C++ (usando PubSubClient para MQTT).

📌 Funcionalidades
- Controle remoto da fechadura via aplicativo web.
- Autenticação de usuários (opcional, se aplicável).
- Logs de acesso em tempo real.
- Notificações (ex: Telegram, e-mail) ao trancar/destrancar.

⚙️ Configuração
1. ESP32
Instale as bibliotecas no Arduino IDE:

```c
#include <WiFi.h>
#include <PubSubClient.h>
```
Configure WiFi e MQTT no arquivo config.h:
```c
#define WIFI_SSID "SUA_REDE"
#define WIFI_PASS "SENHA"
#define MQTT_BROKER "broker.mqtt.com"
```

2. Servidor Node.js
Instale as dependências:
```c
cd server
npm install mqtt express
```

3. Aplicativo Web
Instale as dependências (se usar React/Vue):
```c
cd frontend
npm install
npm start
```

Acesse: http://localhost:3000.
