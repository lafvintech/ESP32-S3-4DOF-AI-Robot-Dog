Introduction
============

Dear friends, welcome to the learning world of the ESP32 S3 4DOF AI robot dog!

Please read this document carefully. If you encounter any problems during use, please contact our after-sales support team at **`support@lafvin.cn` **, and we will assist you as soon as possible.

----

**ESP32 S3 4DOF AI Robot Dog**

.. image:: _static/Introduction/1.board.png
   :width: 600
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

Bill of Materials
-----------------

.. image:: _static/Introduction/2.bom.png
   :width: 600
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. list-table:: 
   :header-rows: 1
   :widths: 10 40 20
   :align: center

   * - Serial Number
     - Name
     - Quantity
   * - 1
     - ESP32-S3 4-DOF AI Robot Dog Control Board
     - x1
   * - 2
     - SG90 Servo
     - x4
   * - 3
     - 0.96-inch OLED Display
     - x1
   * - 4
     - Speaker
     - x1
   * - 5
     - Servo Bracket
     - x4
   * - 6
     - 3D-Printed Part (Leg)
     - x4
   * - 7
     - 3D-Printed Part (Head)
     - x1
   * - 8
     - Type-C Data Cable
     - x1
   * - 9
     - Phillips Screwdriver
     - x1
   * - 10
     - Screw Pack
     - x1
   * - 11
     - Cable Tie
     - x4

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

  - The package does not include an 18650 battery. The Type-C data cable is only for flashing firmware and charging. Please note that powering the entire system solely through the Type-C data cable is insufficient and may cause the robot to crash or restart.
  
  - Please check the contents of the package against the bill of materials. If you find any missing or damaged items, please contact our technical support team immediately.

----

Technical Parameters
--------------------

.. list-table:: 
   :header-rows: 1
   :widths: 20 30
   :align: center

   * - Parameter
     - Value
   * - Input Voltage
     - 3.7V-5V
   * - Operating Voltage
     - 3.3V-5V
   * - Charging Voltage
     - TYPE-C 5V/2A
   * - Main Control Chip
     - ESP32 S3 N16R8
   * - Servo Model
     - SG90 Servo
   * - Screen Model
     - SSD1306 0.96-inch OLED Display
   * - Power Amplifier Chip
     - MAX98357AETE+T
   * - Microphone Model
     - Digital I2S ZTS6672
   * - Speaker
     - 8Ω 2W

.. raw:: html

   <div style="margin-top: 30px;"></div>

Function Introduction
---------------------

**Introduction:**

 - The LAFVIN 4DOF AI Robot Dog is an assembleable intelligent robot dog kit based on the ESP32-S3. 

 - It uses four servo motors to drive its four legs, enabling it to perform a variety of actions such as moving forward, backward, turning, sitting, shaking hands, dancing, and sleeping. 
 
 - It supports Wi-Fi connectivity, voice interaction, web-based remote control, OLED facial expression display, and RGB lighting effects, making it suitable for maker projects, STEM education, and robot programming learning.

**Features:**

- **AI Voice Interaction**

  After connecting to Wi-Fi, it enables voice wake-up and voice dialogue. Users can issue action commands via natural language, such as forward, backward, turn, sit, or perform actions; they can also control screen expressions and RGB lighting effects via voice.

- **Multi-Step Movement Control**

  Supports four basic movement modes: forward, backward, left turn, and right turn. Voice control can recognize step count commands such as "forward 5 steps" and "backward 3 steps"; control can also be completed directly by clicking the direction buttons on the web interface.

- **9 Preset Action Performances**

  Built-in action performances include sitting, stretching, swaying, shaking hands, dancing, being happy, showing off, and sleeping. Different actions are performed through coordinated movement of all four legs, suitable for interactive displays and desktop companionship scenarios.

- **Mobile Web Remote Control**

  After connecting the device to home Wi-Fi, mobile phones, tablets, or computers can access the control page by accessing the device's IP address, without the need for additional app installation. The page allows control of movement direction, action performances, expressions, RGB lighting effects, and servo motor calibration.

- **OLED Expression and Status Display**

  The 0.96-inch OLED screen displays Wi-Fi status, time, battery level, initialization prompts, and dialogue subtitles. In expression mode, it displays dynamic eye expressions such as blinking, happiness, sadness, anger, surprise, thinking, crying, and sleeping.

- **Expression Mode**

  A long press of the BOOT button enters a focused expression display mode, where the screen primarily displays dynamic expressions. When the robot dog performs actions, it can also randomly display matching expressions to enhance interactivity.

- **RGB Ambient Lighting Effects**

  Equipped with two programmable RGB LEDs, it supports six modes: constant light, breathing, rainbow, flowing water, flashing, and motion-linked. In motion-linked mode, the light color and effects change according to the walking or movement rhythm.

- **Servo Zero-Point Calibration**

 The web interface supports individual fine-tuning of each of the four leg servos, increasing or decreasing in 1° increments. The calibrated zero point is automatically applied to the Home posture and all movement trajectories, facilitating adaptation to different installation errors and 3D-printed leg components.

- **Battery Monitoring**

 Real-time monitoring of the voltage of a single 3.7V lithium battery cell, displaying the remaining battery level in the status bar for convenient and timely charging.

- **Open DIY and Secondary Development**

 Based on the ESP32-S3 and open-source ESP-IDF development environment, users can further modify motion angles, web interfaces, screen expressions, lighting effects logic, and voice interaction methods, making it suitable for learning embedded systems, robot control, and AI application development.

----

Resource Download
-----------------

The sample code required for this course has been provided; you can access all the resources via the following link.

.. raw:: html

    <a href="_static/Test_Code.zip" class="btn btn-primary" download>📥 Download Example program</a>
    
----

**Next, we will delve into the core content of the course and help you gradually understand the relevant concepts and master the operation procedures.**

----
