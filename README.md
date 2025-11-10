⚙️ 1. Sensor-Based Detection

IR Receiver:
The IR (Infrared) receiver detects infrared light signals emitted by an IR transmitter or a remote.
When an IR signal is detected, it outputs a LOW (0) signal to the ESP32.

PIR Sensor (Passive Infrared Sensor):
The PIR sensor detects motion by sensing the infrared radiation emitted by human bodies.
When motion is detected, the sensor outputs a HIGH (1) signal.

These sensors act as the input devices for the ESP32.

💡 2. Microcontroller Decision Making (ESP32)

The ESP32 microcontroller processes signals from both sensors.

It checks whether the sensors are detecting any activity and then takes a logical decision to control the output devices (LEDs).

The ESP32 acts as the brain of the system.

🔦 3. Output Actuation

Red LED: Turns ON when the IR receiver detects a signal.

Blue LED: Turns ON when the PIR sensor detects motion.

This output response represents an automation action — like turning on a light, triggering a gate, or alerting a system.

🌐 4. IoT and Embedded Concept

This project demonstrates how embedded systems work:
Input (Sensors) → Processing (ESP32) → Output (LEDs).

It is a foundational example of an IoT node — a small device that collects data and reacts locally.

If extended with Wi-Fi and cloud platforms like ThingSpeak or MQTT, it can send data to the internet, making it a smart IoT system.

⚡ 5. Automation Logic

The project simulates real-world automation concepts like:

Automatic parking gates (IR-based)

Motion-activated lighting or alarms (PIR-based)

This is achieved through digital logic control — turning outputs ON or OFF based on sensor states.

🧩 6. Key Concepts Involved
Concept	Description
Digital Input/Output	Reading digital HIGH/LOW signals from sensors and writing to LEDs
Conditional Logic	Using if conditions in code to respond to sensor input
Embedded System Design	Combining hardware (sensors, LEDs) and software (MicroPython)
Automation	Performing actions without human intervention
IoT Fundamentals	Demonstrates edge sensing and local control
