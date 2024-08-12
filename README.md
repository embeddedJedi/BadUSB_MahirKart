# Example of a well-purposed BadUSB using the HID (Human Interface Device) feature of MahirKart based on RP2040


<p float="left">
  <img src="https://github.com/user-attachments/assets/7a5ab23e-dab1-447d-aca1-fb6f76d29c3e" width="45%" />
  <img src="https://github.com/user-attachments/assets/72b7d9d9-4103-4b5e-b4b9-3305a805af9b" width="35%" />
</p>


---

# Guide

<strong style="color: #388e3c;">Note:</strong> You only need to have one RP2040-based card. In this example it will be done with `MahirKart`.


- <strong style="color: #388e3c;">1.</strong> Plug the device into a USB port while holding the boot button. It will show up as a removable media device named `RPI-RP2`.
  
- <strong style="color: #388e3c;">2.</strong> Install `CircutlPython` on your RP2040-based development board. [Download CircutlPython files here](https://circuitpython.org/board/raspberry_pi_pico/)

- <strong style="color: #388e3c;">3.</strong> Copy the downloaded `.uf2` file to the root of the Pico (`RPI-RP2`). The device will reboot and after a second or so, it will reconnect as `CIRCUITPY`.

- <strong style="color: #388e3c;">4.</strong> Now we need to install the necessary libraries on our device: Download `adafruit-circuitpython-bundle-9.x-mpy-20240730.zip` from [here](https://circuitpython.org/libraries) and extract this file to a folder.

![image](https://github.com/user-attachments/assets/2a9de41d-40e0-409e-ad0b-670d351a0293)

Navigate to lib in the recently extracted folder and copy `adafruit_hid` to the lib folder on your Raspberry Pi Pico.

- <strong style="color: #388e3c;">5.</strong> We need to create the `python` code that we want our card to run every time it starts, in `CircutlPython` the file name should be `code.py` (`main.py` in MicroPython) and save it inside our card.
