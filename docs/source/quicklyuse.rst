LAFVIN 4DOF AI Robot Dog Quick Start Guide
====================================

:Product Version: LAFVIN 4DOF AI Robot Dog v2.0.0
:Controller: ESP32-S3
:For: DIY makers, STEM learners, educators, and robotics enthusiasts

.. contents:: Contents
   :depth: 3
   :local:

Product Overview
----------------

The LAFVIN 4DOF AI Robot Dog is a four-degree-of-freedom smart robot dog DIY kit powered by an ESP32-S3.
Four SG90 micro servos independently drive the front-left, rear-left, front-right, and rear-right legs for walking,
turning, and expressive motion routines.

The robot dog integrates Wi-Fi, AI voice interaction, an OLED animated expression display, a speaker, programmable
RGB lighting, browser-based controls, and battery-level monitoring. You can interact with it by voice or use a phone
browser to control movement, play actions, test OLED expressions, select RGB effects, and calibrate the servo home positions.

.. important::

   This is an assemble-and-adjust robot kit. Servo manufacturing tolerances, servo-horn mounting positions, and
   3D-printed part tolerances can affect its standing and walking performance. Before first use, check the
   ``Home Position`` and complete servo zero-position calibration.


What's in the Box
-----------------

.. list-table::
   :widths: 70 15
   :header-rows: 1

   * - Component
     - Quantity
   * - ESP32-S3 4DOF AI Robot Dog Control Board
     - 1
   * - SG90 Micro Servo
     - 4
   * - 0.96-inch OLED Display
     - 1
   * - Speaker
     - 1
   * - Servo Bracket
     - 4
   * - 3D-Printed Leg
     - 4
   * - 3D-Printed Head
     - 1
   * - USB Type-C Data Cable
     - 1
   * - Phillips Screwdriver
     - 1
   * - Screw Set
     - 1
   * - Cable Tie
     - 4

.. danger::

   **Battery not included.** Use one 3.7 V 18650 lithium-ion cell only. A fully charged cell is approximately 4.2 V.
   Do not connect two cells in series, a 9 V battery, or any voltage above the range of a single lithium-ion cell to
   the ``BAT`` input. Incorrect power wiring can damage the control board, servos, or battery.


Before You Begin
----------------

#. Prepare a level surface with moderate friction. For the first walking test, avoid glass, polished tile, and deep-pile carpet.
#. Confirm that the four servos, 3D-printed legs, servo brackets, and screws are present.
#. Use the included USB Type-C cable to connect the robot dog to a computer for power, firmware flashing, or debugging.
#. Prepare one healthy 3.7 V 18650 lithium-ion cell and verify the battery polarity against the markings on the control board.
#. During the first assembly, do not fully tighten the servo-horn and leg screws until the initial standing pose has been checked.

.. note::

   The OLED battery percentage is an estimate. A small difference from the voltage measured by a multimeter is normal.


Assembly and Leg Installation
-----------------------------

Each servo controls one leg. The left and right legs are mirror-image parts and **must not be swapped**.
Follow the assembly diagram and labels on the control board when connecting the servos.

.. list-table:: Servo Signal Mapping
   :widths: 35 25 40
   :header-rows: 1

   * - Leg Position
     - Signal Pin
     - Abbreviation
   * - Front Left
     - GPIO17
     - LF
   * - Rear Left
     - GPIO18
     - LR
   * - Front Right
     - GPIO13
     - RF
   * - Rear Right
     - GPIO14
     - RR

Recommended assembly order:

#. Fit each SG90 servo into a servo bracket.
#. Secure the brackets to the body structure.
#. Install the 3D-printed legs in their correct left/right mirror orientation.
#. Power on the robot dog and run :guilabel:`Home Position` once.
#. Check that all four feet rest on the surface and that the body is reasonably level.
#. If a leg is raised, leaning too far forward, or leaning too far backward, complete :ref:`servo-calibration-en` first.

.. warning::

   Never force a leg by hand while the servo is powered. If a leg contacts the body, binds mechanically, or a servo
   continues to jitter, stop the action immediately and disconnect power before inspecting the assembly.


Powering On and Connecting to Wi-Fi
-----------------------------------

#. Insert one 18650 cell, or provide stable power through the USB Type-C port.
#. During startup, the OLED displays initialization and Wi-Fi connection status.
#. After the device connects to Wi-Fi, it enters standby mode and briefly displays its IP address below the status bar.
#. Write down this address, for example ``192.168.1.100``.
#. Connect your phone, tablet, or computer to the **same Wi-Fi network** as the robot dog.

In standby mode, the OLED status bar shows:

* Wi-Fi status on the left;
* time in the center; and
* estimated battery level on the right.

.. danger::

   The ESP32-S3 supports **2.4 GHz Wi-Fi only**. The robot dog cannot connect to a 5 GHz-only network. It may also be
   unreachable from a phone connected through a client-isolated guest network.


Web Control
-----------

After confirming that your phone and the robot dog are on the same local network, enter the IP address shown on the OLED
screen in your browser address bar:

.. code-block:: text

   http://192.168.1.100

The ``AI DOG Smart Control`` page provides the controls below.

Movement Controls
^^^^^^^^^^^^^^^^^

* :guilabel:`Forward`: Walk forward.
* :guilabel:`Backward`: Walk backward.
* :guilabel:`Turn Left`: Turn left.
* :guilabel:`Turn Right`: Turn right.
* :guilabel:`Home Position`: Return to the calibrated standing pose.
* :guilabel:`Stop`: Stop the current action and return to a safe pose.

Preset Actions
^^^^^^^^^^^^^^

The web interface includes nine preset actions:

.. list-table::
   :widths: 25 75
   :header-rows: 1

   * - Button
     - Description
   * - ``Sit``
     - Sit down and hold the pose.
   * - ``Stand``
     - Return to the standing pose.
   * - ``Stretch``
     - Perform a synchronized forward-and-backward leg stretch.
   * - ``Sway``
     - Perform a body-swaying action.
   * - ``Dance``
     - Perform a dance routine.
   * - ``Shake Hands``
     - Raise the front-left leg for a handshake.
   * - ``Happy``
     - Perform a happy interaction routine.
   * - ``Showcase``
     - Demonstrate the legs one at a time.
   * - ``Sleep``
     - Move into and hold a sleeping pose.

.. tip::

   ``Sit`` and ``Sleep`` keep the robot dog in their final pose. Before walking again, select :guilabel:`Home Position`
   or :guilabel:`Stand` to prevent the feet from dragging and to improve movement stability.


Voice Control
-------------

Once the device is online and its AI voice service has initialized, use the configured wake word to start an interaction.
If the wake word is not recognized, **short-press the BOOT button** to enter listening mode directly, then speak your command.

Example voice commands:

.. code-block:: text

   Go forward.
   Go forward five steps.
   Go backward three steps.
   Turn left.
   Turn right.
   Sit down.
   Shake hands.
   Dance.
   Show a happy expression.
   Turn on rainbow lights.

Forward and backward commands support step counts. For example, saying ``Go forward five steps`` repeats the appropriate
walking sequence five times.

.. note::

   Voice recognition depends on network quality, ambient noise, speaking distance, and microphone installation.
   For best results, speak clearly, use short commands, and stay close to the robot dog.


OLED Expression Mode
--------------------

In normal mode, the OLED shows Wi-Fi status, time, battery level, dialogue subtitles, and a small expression.
**Long-press the BOOT button** to enter or exit ``Expression Mode``.

In Expression Mode, the screen focuses on animated eye expressions and no longer shows dialogue subtitles. Voice audio
output continues normally. Use the :guilabel:`Expressions` page in the web interface to test the available expressions:

* Neutral, Happy, Sad, Angry, and Surprised;
* Thinking, Sleepy, Winking, and Crying.

When Expression Mode is active, some motion routines also display randomly selected expressions that match the action.


RGB Lighting
------------

Open :guilabel:`RGB Lighting` from the bottom of the web interface to turn RGB effects on or off and select an effect:

.. list-table::
   :widths: 25 75
   :header-rows: 1

   * - Effect
     - Description
   * - ``Solid``
     - Solid white light.
   * - ``Breathe``
     - Breathing light effect.
   * - ``Rainbow``
     - Rainbow color transition.
   * - ``Flow``
     - Flowing light effect.
   * - ``Flash``
     - White flashing light.
   * - ``Motion Sync``
     - Lighting synchronized with walking and servo movement.

When RGB effects are disabled, the LEDs return to their system-status indication function. In ``Motion Sync`` mode,
the LEDs are solid white while idle, then vary in color and flash rate with the movement direction, servo speed, and action rhythm.


.. _servo-calibration-en:

Servo Zero-Position Calibration
-------------------------------

Servo tolerances, servo-horn spline positions, and 3D-printed part tolerances can cause assembly offsets. Use the
:guilabel:`Servo Setup` page to calibrate the Home position of each leg.

#. Select :guilabel:`Home Position` to move the robot dog to its initial standing pose.
#. Check whether all four feet contact the surface and whether the body leans noticeably to one side.
#. Choose the leg to adjust in :guilabel:`Servo Setup`.
#. Use ``−`` or ``+`` to adjust the value in **1° increments**.
#. Select :guilabel:`Apply and Go Home` to check the result.
#. Repeat as needed until all four feet make stable contact and the body is approximately level.

The calibrated zero positions are stored in the device and are applied automatically to the Home pose, walking, turning,
and preset action routines.

.. danger::

   Adjust by only 1--2° at a time and observe the result before making further changes. Large adjustments may cause a leg
   to hit the body, lift a foot off the surface, or stall a servo at its mechanical limit.


Battery and Power Notes
-----------------------

* Use one 3.7 V 18650 lithium-ion cell.
* A fully charged cell is approximately 4.2 V. Low voltage reduces servo torque and Wi-Fi stability.
* If movement becomes weak, servos jitter, the device restarts, or Wi-Fi disconnects, check the battery level first.
* Remove the battery when the product will not be used for an extended period.
* Do not use a damaged, swollen, leaking, or otherwise abnormal battery.

.. warning::

   Servos draw substantial current during movement. Use a sufficiently charged, reliable battery or USB power source.
   Insufficient power can cause OLED flickering, Wi-Fi disconnections, voice failures, or unexpected restarts.


Troubleshooting
---------------

The device will not power on or the OLED stays blank
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Check that the USB Type-C cable and power source are working.
* Check the battery charge level and polarity.
* Remove the battery and test with a stable USB Type-C power source only.

The web control page does not open
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Confirm that the phone and robot dog are connected to the same 2.4 GHz Wi-Fi network.
* Enter the complete address, for example ``http://192.168.1.100``.
* Restart the robot dog and wait for the OLED to show its IP address again.
* Disable VPN on the phone and avoid guest networks with client isolation enabled.

The wake word or voice interaction does not respond
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Confirm that the device is online and has completed startup.
* Short-press BOOT to check whether direct listening mode works.
* Speak near the microphone and away from loud noise sources such as fans, televisions, or crowds.
* Check the speaker connection and power supply.

The robot dog shuffles, walks crookedly, or raises a foot
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Test on a flat, dry surface with moderate friction.
* Check that the battery is sufficiently charged.
* Confirm that the left and right legs are not swapped and that servo connections are correct.
* Recalibrate all four legs as described in :ref:`servo-calibration-en`.
* Check for loose servo-horn, bracket, or leg screws.

The servos jitter continuously or become hot
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* Select :guilabel:`Stop` immediately and disconnect power.
* Check whether a leg is hitting the body, blocked by an object, or at its mechanical limit.
* Check for a low battery.
* Recalibrate the affected leg's Home position to prevent the servo from remaining stalled.


Advanced: Flashing Firmware
---------------------------

For advanced users who need to restore or update the system, a complete merged firmware image is provided in the project root:
``LAFVIN-4DOF-AI-Robot-Dog-v2.0.0-full.bin``.

This is a complete image for an ESP32-S3 with 16 MB flash and must be flashed from address ``0x0``. With ESP-IDF,
run the following command from the project directory:

.. code-block:: console

   idf.py -p COM12 flash

Replace ``COM12`` with the actual serial port used by your computer.

.. warning::

   Before flashing a complete firmware image, verify the chip model, flash size, and flash address. Using an incorrect
   image or flash setting can prevent the device from booting and may erase saved Wi-Fi credentials and servo calibration data.
