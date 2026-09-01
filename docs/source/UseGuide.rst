Function Usage Guide
====================

**This section explains how to use the LAFVIN Desktop AI Gimbal Robot through its main functions and real operating workflows. It covers gesture recognition, OLED display interaction, servo control, Follow this guide when configuring the system, running demos, and troubleshooting common issues to make the most of your robot.**

Intelligent AI Voice Dialogue
-----------------------------

.. image:: _static/function/3.xiaozhi.png
   :width: 600
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

This project is perfectly compatible with Xiaozhi AI and supports multiple languages. You can converse with the robot via voice. The robot will process your voice input and respond accordingly based on your configured settings.

- You can ask it any questions:

 - "What is the weather like today?"
 - "What is the current time?"
 - "What is the current humidity?"
 - "Tell a joke"
 - "What is the capital of France?"
 - "How are you doing?"
 - "What is the meaning of life?"
 - "Tell me a story"
 - "What is your favorite color?"
 - "What is the weather like tomorrow?"
…

- With the servo gimbal, you can also say: 

 - "Shake your head left/right"
 - "Scan left, right, and up."
 - "Shaking head left and right"
 - "Look up"
 - "Nod"
…

.. attention::

 - The factory default wake-up phrase is **Hi，ESP!** .

 - Alternatively, you can start a conversation by briefly pressing the **BOOT** button.

----

Emoticon Mode
-------------

After the robot is powered on, it defaults to conversation mode. You can enter expression mode by long-pressing the **BOOT** button. In this mode, the robot will respond to your voice commands by displaying corresponding emoticons on its OLED screen. This allows for a fun and interactive way to express emotions through the robot. You can switch back to conversation mode by long-pressing the **BOOT** button again.

.. image:: _static/function/4.display.png
   :width: 600
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

- In Emoticon Mode,you can say:

 - "Show me a happy face"
 - "Show me a sad face"
 - "Play badminton animation"
 - "Play Face ID animation"
…

- The following are 41 graphic expressions built into the system. You can directly say:

.. image:: _static/function/1.biaoqinji.png
   :width: 400
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

- For example: **Play Rainy animation**, and the system can play the corresponding graphic expressions.

----

Gesture Recognition
-------------------

.. image:: _static/function/2.gesture.png
   :width: 600
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

This robot is equipped with a gesture recognition system that understands and responds to specific gestures. With this feature, you can control the gimbal's direction without using voice commands. You can make various gestures in front of the gesture recognition module, and it will recognize and execute the corresponding functions.

- Supported gestures include:

- "Swipe left"

- "Swipe right"

- "Swipe up"

- "Swipe down"

- "Circle clockwise"

- "Circle counterclockwise"

- "Push palm forward"

- "Push palm forward"

- "Quick wave"

For example, you can swipe left to turn the gimbal to the left, or draw a circle clockwise to display various expressions on the OLED screen. The gesture recognition system provides an intuitive way to interact with the robot and control its behavior in real time.

.. attention:: 

  To ensure accurate recognition by the PAJ7620U2 module when making gestures, please note the following:

 - Control the distance: Place your hand 5cm to 15cm directly above the sensor. Too close or too far will easily lead to recognition failure.

 - Control the speed: The movement should be crisp and steady. Avoid moving too slowly (like a snail's pace), but a normal speed is sufficient; extreme speed is unnecessary.

 - Complete the circles: When making clockwise or counterclockwise gestures, at least two complete circles need to be completed consecutively.

 - Distinguish between "forward" and "backward": This refers to vertical pushing/pulling (approaching/moving away from the sensor), not horizontal sliding.

 - Avoid strong light: Avoid using the device in direct sunlight or under strong lights to prevent interference with the infrared signal.

----

FAQ For Function Usage Guide
----------------------------

**​How ​​to switch operating modes after powering on?**

- Press and hold the **BOOT** button to switch between Conversation mode and Emoticon mode. Powering on defaults to Conversation mode.

----

**What to do if voice commands are not recognized or are unresponsive?**

- Check if the network or voice service (such as Xiaozhi AI) is available and correctly configured.

- Speak in a quiet environment to avoid excessive background noise.

- If there is still no response, restart the device and check the serial port/log for error information.

----

**How ​​to improve the recognition rate when gesture recognition frequently fails?**

- Please refer to the precautions in the gesture recognition section:

- Place your hand 5–15cm above the sensor; too close or too far will affect recognition.

- Move your hand decisively and at a moderate speed; circular gestures require at least two consecutive circles.

- Avoid direct sunlight on the sensor; keep the sensor surface clean.

----

**What to do if the OLED screen does not display or displays abnormally?** 

- Check that the power supply and connection cables are secure.

----

**How ​​to troubleshoot servo motors that are not moving or vibrating?**

- Ensure the power supply provides sufficient current (do not rely solely on USB power when operating multiple servos).

- Check that the servo signal cables and wiring sequence are correct.

- If the position is off or stuck, perform servo limit/zero point calibration and check the mechanical limits.

----

**How ​​to make the robot execute voice commands such as head shaking?**

- Use example phrases directly in conversation mode (e.g., "Shake your head left/right", "Scan left, right, and up").

----

**How ​​to restore factory settings or reset the device?**

- This document does not define a one-button restore procedure. To clear the configuration, you can re-flash the factory firmware.

----

**Which languages ​​are supported?**

- This project is compatible with Xiaozhi AI and supports multiple languages. Specific supported languages ​​depend on the configured voice service and model.

----

**What safety precautions should be taken when using the device?**

- Avoid touching the servos directly with your hands while they are moving.

- Do not use the equipment in high temperature or humid environments. Avoid water ingress and short circuits.

- Do not apply additional loads to the servo motor or force it to move beyond its mechanical limits.

----