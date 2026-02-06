# MakeOhio

Hardware + software hackathon project built at MakeOhio. Combines an Arduino Mega microcontroller with a MERN stack web dashboard for real-time monitoring and control.

## Architecture

```
Hardware/     # Arduino Mega (PlatformIO) — RFID, RTC, LCD, sensors
Software/     # MERN stack web dashboard
  mern/
    client/   # React + Vite frontend (Tailwind CSS)
    server/   # Express + MongoDB backend
```

## Hardware

- **Platform**: Arduino Mega 2560 (PlatformIO)
- **Components**: MFRC522 RFID reader, RTC clock, LCD display, Servo motor
- **Libraries**: Adafruit BusIO, RTClib, LiquidCrystal, MFRC522

## Software

- **Frontend**: React, Vite, Tailwind CSS, Cypress (E2E tests)
- **Backend**: Express.js, MongoDB
- **CI/CD**: GitHub Actions

## Getting Started

### Web Dashboard

```bash
cd Software/mern/client
npm install
npm run dev
```

```bash
cd Software/mern/server
npm install
node server.js
```

### Hardware

Open `Hardware/` in PlatformIO and upload to an Arduino Mega 2560.
