# cleaning_bot_usingArduino
# 🧹 Cleaning Bot

A smart, Arduino-powered cleaning robot that follows user-defined paths or navigates autonomously using obstacle avoidance. Built with simple yet powerful components like HC-05 Bluetooth, L298N motor driver, and ultrasonic sensors, Cleaning Bot is a flexible, efficient solution for modern households and small businesses.

![Cleaning Bot Demo](images/bot_demo.jpg)

---

## 🔧 Features

- 📱 **Bluetooth Control** via HC-05 module
- 🧭 **Custom Path Cleaning** using directional commands
- 🤖 **Automatic Mode** with real-time obstacle avoidance
- 🧠 **Path Memory** with reverse navigation support
- ⚙️ **Dual Motor Control** using L298N driver
- 🛠️ Easy to build and modify for DIY enthusiasts

---

## 🧰 Hardware Components

| Component           | Description                     |
|--------------------|---------------------------------|
| Arduino UNO        | Main microcontroller            |
| HC-05 Module       | Bluetooth communication         |
| L298N Motor Driver | Dual DC motor control           |
| 2x DC Motors       | Drive system                    |
| Ultrasonic Sensor  | Obstacle detection              |
| Chassis + Wheels   | Physical body of the robot      |
| Power Supply       | Battery or external power       |

---

## 🔌 Circuit Diagram

![Circuit Diagram](images/circuit_diagram.png)

---

## 🧠 How It Works

- **Manual Mode**: Control the bot using F (forward), B (backward), L (left), R (right), 0 (stop), and X (reverse path).
- **Automatic Mode**: Entered using 'T'. The bot automatically detects and avoids obstacles using the ultrasonic sensor.
- **Reverse Navigation**: After path completion, press 'X' to retrace steps back to the start.

---

## 📜 Code Overview

The Arduino sketch uses:
- `Serial.read()` to receive Bluetooth commands
- Motor control logic with `digitalWrite()`
- Path storage and reversal logic using a `char[]`
- Obstacle avoidance with ultrasonic distance measurements

> 📂 Code is located in `code/cleaning_bot.ino`.

---

## 🚀 How to Use

1. Upload the sketch to Arduino UNO.
2. Power the bot and pair the HC-05 module via your phone.
3. Use a Bluetooth terminal app to send commands:
   - `F` – Forward
   - `B` – Backward
   - `L` – Left
   - `R` – Right
   - `0` – Stop
   - `X` – Retrace path
   - `T` – Start automatic obstacle mode
   - `S` – Exit automatic mode

---

## 📽️ Demo

> 🎥 Add a short video or GIF here showing the bot cleaning a space manually and automatically.

---

## 🛠️ Future Improvements

- Add live path visualization via mobile app
- Integrate voice assistant control
- Upgrade to GPS for large-scale area mapping

---

## 📄 License

This project is currently unlicensed. You may modify and share the code at your own discretion.

---

## 🤝 Contributing

Feel free to open issues or submit pull requests if you want to improve the bot or its documentation.

---

## 📬 Contact

For any queries or suggestions, reach out via GitHub Issues.


