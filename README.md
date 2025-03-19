# 🔆 Arduino Sequential Blinking Lights

This project demonstrates how to sequentially turn on and off **three LEDs** using an **Arduino**. It is a great way to learn about digital output control and timing using **delay()**.

## ✨ Features
- Sequentially blinks **three LEDs** in a loop.
- Demonstrates the use of **digitalWrite()** and **delay()**.
- Simple setup, ideal for beginners.
- Customizable timing for different effects.

## 🛠️ Requirements
- **Arduino board** (Uno, Nano, or compatible)
- **3 LEDs** (any color)
- **3 Resistors** (220Ω recommended)
- **Jumper wires**
- **Breadboard**

## 🔧 Setup
1. **Connect LEDs**:
   - LED1 → Pin **13**
   - LED2 → Pin **12**
   - LED3 → Pin **11**
2. Attach a **220Ω resistor** in series with each LED.
3. Connect the **other end of each LED to GND**.
4. Upload the Arduino sketch to your board.

## 📜 Code Example
```cpp
int LED1 = 13;
int LED2 = 12;
int LED3 = 11;

void setup() {
  pinMode(LED1, OUTPUT);
  pinMode(LED2, OUTPUT);
  pinMode(LED3, OUTPUT);
}

void loop() {
  digitalWrite(LED1, HIGH);
  delay(200);
  digitalWrite(LED2, HIGH);
  delay(200);
  digitalWrite(LED3, HIGH);
  delay(200);
  digitalWrite(LED1, LOW);
  delay(300);
  digitalWrite(LED2, LOW);
  delay(300);
  digitalWrite(LED3, LOW);
  delay(300);
}
```

## 🎛️ Customization
- Change the **LED pins** to use different digital pins.
- Adjust **delay()** values to modify the blinking speed.
- Add more LEDs for a **longer sequence**.

## 🤝 Contributing
Feel free to **fork**, modify, and submit pull requests to enhance the project!

Enjoy experimenting with LEDs! 💡⚡
