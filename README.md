# snake-balls
This is a bio-inspired snake robot designed for the **Hack Club Stack** challenge.  while relying on a minimalist hardware and code setup.

## How It Works (Mechanical + Code)
- **One Motor, One Wheel Propulsion:** The robot is driven by exactly **one  TT DC motor connected to a drive wheel**. 

- **Autonomous Start/Stop:** The code strictly handles obstacle avoidance. The Raspberry Pi Pico reads the distance from the front ultrasonic sensor:
  - **PATH CLEAR:** Motor starts and drives forward.
  - **OBSTACLE AHEAD (< 20cm):** Motor stops completely to prevent a collision.

## Hardware Wiring Configuration
To verify the electronics integration, the components are wired directly to the Raspberry Pi Pico as follows:

| Component | Pico Pin | Function |
| :--- | :--- | :--- |
| **HC-SR04 Trigger** | GPIO 3 | Transmit Ultrasonic Pulse |
| **HC-SR04 Echo** | GPIO 2 | Receive Echo Pulse |
| **DRV8833 IN1** | GPIO 14 | Motor Drive Signal (Single Motor) |
| **DRV8833 IN2** | GPIO 15 | Motor Ground/Direction (Single Motor) |

## Project Structure
  - i made the project on cad on shape i puted all the parts inside the main body because i want a beatiful shape
  - i get and made hte code from some tutorials on youtube with a little help from the ai with movement
