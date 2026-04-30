# line-follower-bot-
Built a Line Following Bot for Meshmerize at IIT Bombay using an Arduino Nano, PID logic, and a 7-channel sensor array.
Project Overview
Built specifically for the Meshmerize competition at IIT Bombay, this project is a fully autonomous line-following robot engineered from scratch. The primary challenge of the competition was designing a bot capable of navigating highly complex tracks with both precision and speed. Successfully handling sharp turns without losing the track required extensive hours of testing, tweaking, and debugging the control logic, but seeing it run smoothly made every second worth it.

Hardware Specifications
The brain of the robot is an Arduino Nano (ATmega328P) microcontroller. For precise path detection, the bot utilizes a 7-channel analog sensor array. Mobility is provided by three N20 12V 300RPM Micro Metal Gear Motors equipped with encoders, which are driven by dual TB6612FNG motor drivers for exact speed and direction control. The entire system is efficiently powered by two Flipo 1000mAh 3S 11.1V LiPo batteries.

Software and Control Logic
The navigation code is built around a custom Proportional-Derivative (PD) control system. Instead of relying on hardcoded sensor values, the bot features an auto-calibration sequence that dynamically reads ambient light to establish perfect thresholds for line detection. The sensors use weighted error calculations to determine exactly how far off-center the bot is. The PD control loop then computes the necessary motor adjustments for smooth, jitter-free movement. Furthermore, the bot features adaptive speed control—automatically decelerating when outer sensors detect an upcoming sharp turn—and a line-lost memory system that remembers the last known direction of the track and aggressively rotates the bot back into position if it ever veers off course.

Acknowledgements
This project was a massive collaborative effort. A huge shoutout goes to my amazing teammates Yogita, Amogh Betageri, and Deep for their dedication and teamwork. Special appreciation goes to Dr. Vinayak N Kulkarni sir for his constant support and guidance throughout this journey. Competing at IIT Bombay was an incredible experience that provided fantastic exposure to the level of talent and innovation within the engineering community.
