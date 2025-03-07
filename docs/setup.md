# Kurulum Rehberi

## 1. Donanım Bağlantıları
- ESP32-CAM ↔ RPi Pico: UART veya WebSocket.
- L298N Motor Sürücü ↔ Pico: GPIO2 ve GPIO3.

## 2. Yazılım Kurulumu
- Arduino IDE'yi indirin.
- ESP32 ve Pico için board desteğini ekleyin.
- Gerekli kütüphaneleri yükleyin:
  ```bash
  git clone https://github.com/zuzu-robot/zuzu-libs.git