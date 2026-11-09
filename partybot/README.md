# PartyBot: a gesture-controlled mecanum robot

**Timuçin Topcu, Emre Ertürk, Onur Kansoy, Tarık Yaraşlı** · CENG 424 Embedded Computer Systems, İzmir Institute of Technology, Spring 2026

**[📄 Slides](presentation.pdf)** · **[▶ Demo video](demo.mp4)**

<p align="center"><img src="preview.webp" width="420" alt="PartyBot driving"></p>

Most entertainment props sit in one place and respond to a single button press. PartyBot is a mobile
platform that the user drives continuously with hand movements.

- **Wearable controller.** A glove with kinematic sensors and push buttons on an ESP32 DevKit V1. It
  reads and filters the sensor data, interprets gestures and sends command packets.
- **Link.** ESP-NOW, a low-latency peer-to-peer protocol between the two ESP32s that needs no external network.
- **Robot.** A mecanum-wheel base on a second ESP32 that drives and strafes, plays music, and shows
  expressions on a dot-matrix display, with basic fail-safes.
