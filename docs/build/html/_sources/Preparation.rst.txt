1. Flash The Firmware
=====================

**This product was not pre-programmed at the time of shipment. To use it, you will need to flash the program yourself. Please follow the instructions below to complete the flashing process.**

Online Flashing
---------------

- This method allows you to flash the program directly through the online platform without needing to install any additional software on your computer. It is a convenient option for users who prefer a straightforward flashing process.

- Please watch the video below first to learn how to flash the firmware to the main control board：

.. video:: _static/flash/flash.mp4
    :width: 100%

----

**Below is a detailed step-by-step tutorial with images.**

Step 1: Connect the Device
~~~~~~~~~~~~~~~~~~~~~~~~~~

Use the provided Type-C data cable to connect the **ESP32 S3 4DOF AI Robot Dog** to your computer.

.. image:: _static/flash/9.type-c.png
   :width: 400
   :align: center

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

   After inserting the data cable, you need to turn on the power switch.

----

Step 2: Access the Online Flashing Platform
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Click here to jump directly to the online flashing page: `LAFVIN Web Flasher <https://lafvintech.github.io/Lafvin_Web_Flasher/>`_

.. image:: _static/flash/1.webflash.png
   :width: 800
   :align: center

----

Step 3: Connect Serial Port
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Click "Connect," and in the pop-up serial port selection window, select the appropriate serial port to establish the connection.

.. image:: _static/flash/2.port.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

 If you are unsure which serial port to select, you can disconnect the device and check which port disappears from the list, then reconnect it and select that port.

 If a new serial port is not detected, it indicates that the main control board has not entered download mode. Please follow these steps: press and hold the **BOOT button**, connect the data cable to the main control board, and then release the **BOOT button**; the corresponding port should then be recognized.

----

Step 4: Select the Firmware
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Select the corresponding firmware as shown in the images below.

.. image:: _static/flash/5.固件.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. image:: _static/flash/6.固件.png
   :width: 800
   :align: center   

----

Step 5: Start Flashing
~~~~~~~~~~~~~~~~~~~~~~

Click the "Flash" button to start the flashing process. The progress will be displayed on the screen, and once completed, you can disconnect the device and start using it.

.. image:: _static/flash/7.烧录.png
   :width: 800
   :align: center   

.. raw:: html

   <div style="margin-top: 30px;"></div>

.. image:: _static/flash/8.烧录.png
   :width: 800
   :align: center   

.. attention::

   The flashing process is only considered complete once the message **Flashing complete! Restoring serial connection. Device ready** appears.

----

FAQ For Flashing Program
------------------------

If you encounter issues with flashing or the flashing process fails, please perform the following self-check steps:

1. **Check USB Connection**: Ensure the Type-C data cable is securely connected to both the ESP32 S3 4DOF AI Robot Dog and your computer. Try using a different USB port or cable if possible.

.. raw:: html

   <div style="margin-top: 30px;"></div>

2. **Verify Power Supply**: Ensure that the device is properly powered on. Please insert an 18650 battery; the main control board must maintain a stable power supply throughout the flashing process.

.. raw:: html

   <div style="margin-top: 30px;"></div>

3. **Check Device Drivers**: Ensure that the necessary USB drivers are installed on your computer. For Windows, check Device Manager for any unrecognized devices. For macOS/Linux, verify serial port permissions.
 
.. raw:: html

   <div style="margin-top: 30px;"></div>

4. **Select Correct COM Port**: In the Flash Download Tool or online flasher, confirm that the correct COM port (serial port) is selected. You can find this in your computer's Device Manager (Windows) or System Report (macOS).
 
.. raw:: html

   <div style="margin-top: 30px;"></div>

5. **Restart Software and Device**: Close the flashing software, disconnect and reconnect the device, then restart the flashing process.
 
.. raw:: html

   <div style="margin-top: 30px;"></div>

6. **Disable Antivirus/Firewall**: Temporarily disable any antivirus software or firewall that might be interfering with the flashing process.

.. raw:: html

   <div style="margin-top: 30px;"></div>

7. **Try Different Browser/Computer**: If using the online flasher, try a different web browser or computer to rule out compatibility issues.
 
.. raw:: html

   <div style="margin-top: 30px;"></div>

8. **Check Firmware File**: Ensure you are using the correct firmware file from the provided resource package and that it is not corrupted.
 
.. raw:: html

   <div style="margin-top: 30px;"></div>

.. attention::

 If the issue persists after performing these checks, please contact our technical support team with details about your setup, error messages, and the steps you've already tried.

----