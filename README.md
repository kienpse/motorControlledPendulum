## Servo Pendulum Control Simulation

This is a single-file HTML simulation designed to demonstrate the fundamentals of controlling an unstable system—specifically, balancing a single pendulum in the inverted (vertical-up) position using a **PID controller**.

### Requirements to Run

This simulation is entirely self-contained within one HTML file. It requires **no server setup, no external libraries, and no special software.**

* **To Run:** You only need a standard **Web Browser** (like Chrome, Firefox, or Edge).
* **To Edit:** Any plain **Text Editor** (like Notepad) is sufficient to view and modify the code.

### How to Use

1.  Copy the code and save it as an `.html` file (e.g., `pendulum.html`).
2.  Double-click the file to open it in your web browser.

### Key Simulation Functions

1.  **Set Initial Angle:** Use the input box to define the pendulum's starting position (where $0^\circ$ is vertical up). Click "Set & Reset" to apply.
2.  **Start/Stop Motor:** This button toggles the control system. When the motor is **ON**, the PID algorithm calculates the required torque. When **OFF**, the pendulum swings freely under gravity.
3.  **PID Tuning ($K_p, K_i, K_d$):** Use the sliders to adjust the Proportional, Integral, and Derivative gains in real-time. This allows you to observe the effects of tuning on stability, speed, and oscillation.

### The Actuator Signal

The PID controller's output is the **Actuator Signal**, which is displayed as the **Motor Torque**. This value is the final command sent to the simulated servo motor. It is calculated as the sum of the $P$, $I$, and $D$ contributions: $\text{Torque} = K_p \cdot \text{Error} + K_i \cdot \text{Integral} + K_d \cdot \text{Derivative}$. 

***
