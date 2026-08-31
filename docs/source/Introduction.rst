Introduction
============

**Dear friends, welcome to the learning world of the ESP32 S3 4DOF AI Robot Dog!**

**Please read this documentation carefully. If you encounter any problems during use, please contact our after-sales support team, and we will assist you as soon as possible.**

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

  - Due to international shipping restrictions, batteries are not included; you will need to purchase one 18650 battery separately for this kit.
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

- This is a multi-functional development board expansion breakout board designed for developers, electronics enthusiasts, and educational experiments. It quickly expands the GPIO, power, and ground resources of commonly used development boards, facilitating the connection of sensors, actuators, display modules, and various electronic experimental components.

- The product features a universal design, supporting various 100mil (2.54mm) standard dual-row pin development boards with widths ranging from 600mil to 1000mil (15.24mm to 25.4mm), and is compatible with common development platforms such as Arduino Nano, ESP32, ESP8266, and Raspberry Pi Pico.

- With onboard power input, power switch, power indicator, GPIO status indicator, and various expansion interfaces, it makes setting up development board experiments simpler, safer, and more efficient.

**Features:**

- **Universal Compatibility Design, Adaptable to Multiple Development Boards**

 - Utilizes a wide-compatible interface design, supporting 100mil (2.54mm) dual-row pin development boards with widths of 600mil, 800mil, 900mil, and 1000mil.

 - Compatible with Arduino Nano, ESP32, ESP8266, Raspberry Pi Pico series, and other standard dual-row pin development boards. No complex adapters are required for quick expansion, meeting the development needs of various projects.

- **Abundant GPIO Expansion, Quick Connection to Peripheral Modules**

 - Through onboard expansion interfaces, the development board's GPIO, power, and ground wires are fully exposed, including: GPIO signal interfaces, 3.3V power supply, 5V power supply, and GND ground.

 - Also provides two-sided screw terminal interfaces, standard female header interfaces, and pin header expansion interfaces, supporting DuPont wire connections, breadboard experiments, and fixed wiring, making experimental setup more flexible and convenient.

- **Independent Indicator Light Design**

 - Onboard power LED indicator displays the current power supply status in real time, allowing for quick and easy determination of system functionality.

 - It also features GPIO status indicator lights, displaying high and low level changes of corresponding I/O ports, facilitating program debugging, signal detection, and hardware verification, making electronic experiments more intuitive.

.. image:: _static/Introduction/3.led.png
   :width: 800
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

- **Added Power Switch for Enhanced Safety and Convenience**

 - Compared to ordinary expansion boards, this product adds an independent ON/OFF sliding power switch, allowing control of the entire experimental system's power supply without frequent power plugging and unplugging. This enables quick power-off during program debugging, prevents accidental operation when modifying circuits, extends interface lifespan, and improves the development experience.

**Target audience or scenarios** 

- Suitable for electronics enthusiasts, students, teachers, makers, and embedded developers. It can be widely used in experiments with Arduino, ESP32, Raspberry Pi, Pico, and other development boards; IoT project development; robot building; smart home construction; STEM education; and electronic prototyping.

- Through convenient GPIO expansion and flexible connection methods, it helps users quickly build experimental circuits, improving development efficiency and suitable for various application needs from beginner learning to professional project development.

----

Resource Download
-----------------

The sample code required for this course has been provided; you can access all the resources via the following link.

.. raw:: html

    <a href="_static/Test_Code.zip" class="btn btn-primary" download>📥 Download Example program</a>
    
----

**Next, we will delve into the core content of the course and help you gradually understand the relevant concepts and master the operation procedures.**

----
