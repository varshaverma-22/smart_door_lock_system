# Self-Driving Bot using Arduino

## Project Overview
This project is a self-driving robot developed using Arduino. It is capable of obstacle detection and autonomous navigation using ultrasonic and IR sensors. The robot uses four DC motors for movement, controlled via the Adafruit Motor Shield.

## Features
- Obstacle detection using an ultrasonic distance sensor.
- Line and edge detection using IR sensors.
- Automatic forward, backward, left, and right movements.
- Servo motor for initial scanning (optional extension for dynamic scanning).

## Components Used
- Arduino Uno
- Adafruit Motor Shield (AFMotor Library)
- 4 DC Motors
- 1 Servo Motor
- Ultrasonic Sensor (HC-SR04)
- 2 IR Sensors (for left and right detection)
- Jumper wires, breadboard, power source

## Circuit Connections
- **Motors:** Connected to motor ports 1, 2, 3, 4 on the Motor Shield.
- **Servo:** Connected to Digital Pin 10.
- **Ultrasonic Sensor:** Trigger - A2, Echo - A1.
- **IR Sensors:** LEFT - A0, RIGHT - A3.

## Code Flow
1. Servo motor sweeps initially (for scanning setup).
2. Continuously reads distance and IR sensor values.
3. Movement decisions:
   - Move forward if both IR sensors are active and no close obstacle.
   - Turn right or left based on IR sensor status.
   - Stop or move backward if an obstacle is detected within a critical range.

## How to Run
1. Connect all components as per the circuit.
2. Upload the Arduino code to your board.
3. Power the robot.
4. The robot will start moving and avoiding obstacles automatically.

## Future Improvements
- Dynamic servo scanning in real-time.
- Advanced pathfinding algorithms.
- Integration with Bluetooth or Wi-Fi for manual override control.

---

### Made by Varsha Verma
