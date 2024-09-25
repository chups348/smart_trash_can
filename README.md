# smart_trash_can
Smart Trash Can 

# Overview
The Smart Trash Can project is an Arduino-based automated trash can that uses an ultrasonic sensor to detect when someone is nearby and opens the lid automatically. This improves hygiene and convenience by reducing the need to touch the trash can lid.

# Components
- Arduino board
- Servo motor
- Ultrasonic sensor (HC-SR04)
- Jumper wires
- Breadboard

# Pin Configuration
- Servo Motor:
  - Control Pin: 9
- Ultrasonic Sensor:
  - Trig Pin: 5
  - Echo Pin: 6

 # How It Works
 1. Distance Measurement:
    - The ultrasonic sensor sends a sound wave at 40,000Hz and measures the time it takes for the echo to return.
 2. Lid Control:
    - The servo motor opens the lid, by rotating 90 degrees if the distance to the object is less than or equal to the threshold value.
    - The lid remains open for 3.5 seconds before closing, allowing the user to insert an object into the can.
    - The servo motor detaches when the lid is closed to save power.
