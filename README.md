# Smart Billing Cart

## Overview

The **Smart Billing Cart** is an embedded system designed to revolutionize retail shopping by automating the billing process. It integrates product identification via RFID and real-time weight verification, ensuring secure, accurate, and convenient checkouts. A custom Android app facilitates billing and payment through a QR code system, improving efficiency and minimizing human interaction at checkout.

## Team Members

- K Vijay Krishnan (U2201115)
- Keziah Mariam Varughese (U2201117)
- Maria Siju Joseph (U2201126)
- Milan Thomas C (U2201133)

**Guide**: Ms. Soni Monica  
**Institution**: Rajagiri School of Engineering & Technology, Department of ECE

---

## Objectives

- Design and implement a smart cart with ESP32, EM-18 RFID reader, HX711 load cell, and 16x2 LCD display.
- Validate items by comparing scanned RFID data with real-time weight.
- Develop an Android app for real-time billing and secure QR code-based payment.
- Prevent billing errors and theft through dual-layer authentication.
- Improve shopping experience by reducing checkout times and enhancing reliability.

---

## Hardware Components

| Component                     | Function                                |
|------------------------------|-----------------------------------------|
| ESP32                        | Controls hardware & communication       |
| EM-18 RFID Reader            | Scans RFID tags on products             |
| HX711 Load Cell + Amplifier  | Measures item weight                    |
| 16x2 LCD + I2C Interface     | Displays product and status info        |
| RFID Tags                    | Uniquely identify items                 |

---

## Software Stack

- **Arduino IDE** – Embedded programming for ESP32
- **XAMPP + PHP** – Backend server and database
- **Android Studio** – Android app for cart interaction and checkout
- **Wi-Fi** – Communication between ESP32 and Android app/server

---

## Features

- Real-time RFID + weight-based item validation  
- Dual-layer verification to reduce fraud  
- Android app with dynamic cart and QR code payment  
- PHP/MySQL product database  
- LCD-based feedback and alerts on cart

---

## System Workflow

1. **Scan Product** → EM-18 RFID reader detects product tag.
2. **Weigh Product** → HX711 load cell measures actual weight.
3. **Verify** → System compares scanned item to stored database.
4. **Add/Remove Item** → Based on scan parity (odd=add, even=remove).
5. **Checkout Enabled** → Only when total weight matches stored weights.
6. **Pay via QR Code** → Checkout completed through Android app.

---

## Challenges Faced

- Weight sensor calibration accuracy
- ESP32-server communication under weak Wi-Fi
- Power supply stability across components
- Real-time sync between hardware and mobile interface

---

## Results

- Accurate item detection and real-time billing
- Efficient checkout process via Android app
- Anti-theft validation using weight mismatch detection
- Total cost: ~ ₹2500 for prototype implementation

---

## Future Enhancements

- Visual item detection via AI and image recognition
- Cloud-based database for scalability
- Multilingual app interface and loyalty program integration
- Enhanced fraud detection via smart sensors
- More payment options like NFC, wallets, or voice payments

---


