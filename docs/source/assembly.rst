2. Assembly Tutorial
====================

**This chapter will explain the assembly process of the AI Robot Dog and provide video and text tutorials, which you can choose to view according to your needs.**

.. attention::

      Before starting the assembly, please make sure to read the instructions carefully and follow the steps in order. If you encounter any issues during the assembly process, feel free to reach out to our support team for assistance. We are here to help you every step of the way!    
            
      Before assembly, please make sure to flash the program onto the main control board to ensure that subsequent servo calibration can proceed normally. If you have not yet completed the flashing process, please refer to the `Flashing Program <FlashingProgram.html>`_ chapter for detailed instructions on how to flash the firmware onto the main control board.

----

Before You Begin
----------------

#. Prepare a level surface with moderate friction. For the first walking test, avoid glass, polished tile, and deep-pile carpet.
#. Confirm that the four servos, 3D-printed legs, servo brackets, and screws are present.
#. Use the included USB Type-C cable to connect the robot dog to a computer for firmware flashing, or debugging.
#. Prepare one healthy 3.7 V 18650 lithium-ion cell and verify the battery polarity against the markings on the control board.
#. During the first assembly, do not fully tighten the servo-horn and leg screws until the initial standing pose has been checked.

----

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

----

**Video Tutorial**

.. video:: _static/assembly/LA076_ROBOT_V2.mp4
    :width: 100%

----

**Illustrated Tutorial**

- The illustrated tutorial provides a step-by-step guide with images to help you through the assembly process. Each step is accompanied by detailed instructions and visuals to ensure that you can easily follow along.

Step 1: Assemble the servo
---------------------------

**Required components:**

- SG90 servo motors (4 PCS)

- Metal servo bracket

- M2 x 10mm screws (8 PCS)

**Assembly Steps:**

- Attach the SG90 servo motors to the metal servo bracket using the M2 x 10mm screws. Ensure that the servo motors are securely fastened and aligned properly.

.. image:: _static/assembly/1.assemble_servo.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

  The servo motors are installed in two different directions: one group for the front legs and one group for the rear legs.

.. image:: _static/assembly/2.assemble_servo.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

Step 2: Assemble the servo motor into the body
------------------------------------------------

**Required components:**

- Assembled servo motor (4 PCS)

- Main control board

- M2 x 10mm screws (8 PCS)

**Assembly Steps:**

- Secure the servo motors to the main control board using the M2 x 10mm screws. Ensure that all screws are tightened properly to prevent any movement during operation.

- Insert the assembled servo motors into the designated slots on the main control board. Make sure that the servo motors are oriented correctly and that the wires are not pinched or obstructed.

.. image:: _static/assembly/3.assemble_servo.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

Step 3: Assemble the swing arm to the leg
-----------------------------------------

**Required components:**

- Servo arm (4 PCS included in the servo package)

- Leg 3D printed parts (4 PCS)

- M1.5x5mm self-tapping screws (4 PCS)

**Assembly Steps:**

- Use M1.5x5mm self-tapping screws to attach the 3D-printed leg parts to the servo arm.

.. image:: _static/assembly/4.assemble_leg.png
   :width: 800
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

Step 4: Assemble the leg to the servo
-------------------------------------

**Required components:**

- Assembled leg (4 PCS)

- M2x4mm screws (4 PCS included in the servo package)

**Assembly Steps:**

- Make sure the firmware has been flashed onto the main control board, install a battery, turn on the switch, and you should see the servo motor rotate back to its initial position.

- Use M2x4mm screws to attach the assembled leg to the servo motor. Ensure that the leg is securely fastened and can move freely without obstruction.

- The legs are initially installed at a 90-degree angle to the horizontal plane.

.. image:: _static/assembly/5.assemble_leg.png
   :width: 800
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

 - If the servo motor does not return to its initial position, please check if the firmware has been flashed correctly. If the issue persists, please contact our support team for assistance.

----

Step 5: Assemble the speaker
----------------------------

**Required components:**

- Speaker (1 PCS)

-Round double-sided tape (1 PCS)

**Assembly Steps:**

- Use round double-sided tape to fix the speaker to the designated position on the main control board and insert the speaker interface into the hole.

.. image:: _static/assembly/5.assemble_leg.png
   :width: 800
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

Step 6: Assemble the screen
---------------------------

**Required components:**

- 0.96" OLED Screen (1 PCS)
- 3D printed head parts (1 PCS)
- M2x10mm screws (4 PCS)
- M2 nuts (4 PCS)

**Assembly Steps:**

- Use M2x10mm screws and M2 nuts to attach the 0.96" OLED screen to the 3D-printed head parts. Ensure that the screen is securely fastened and properly aligned.

- Insert the assembled screen into the designated slot on the main control board. Make sure that the screen is oriented correctly.

.. image:: _static/assembly/6.assemble_screen.png
   :width: 800
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

----

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

----

FAQ For Assembly
----------------

