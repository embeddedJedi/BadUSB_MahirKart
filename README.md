# Example of a well-purposed BadUSB using the HID (Human Interface Device) feature of MahirKart based on RP2040


<p float="left">
  <img src="https://github.com/user-attachments/assets/7a5ab23e-dab1-447d-aca1-fb6f76d29c3e" width="45%" />
  <img src="https://github.com/user-attachments/assets/72b7d9d9-4103-4b5e-b4b9-3305a805af9b" width="35%" />
</p>


---

# Quick Guide

<strong style="color: #388e3c;">Note:</strong> You only need to have one RP2040-based card. In this example it will be done with [`MahirKart`](https://mahirkart.net/).


- <strong style="color: #388e3c;">1.</strong> Plug the device into a USB port while holding the boot button. It will show up as a removable media device named `RPI-RP2`.
  
- <strong style="color: #388e3c;">2.</strong> Install `CircutlPython` on your RP2040-based development board. [Download CircutlPython files here](https://circuitpython.org/board/raspberry_pi_pico/)

- <strong style="color: #388e3c;">3.</strong> Copy the downloaded `.uf2` file to the root of the Pico (`RPI-RP2`). The device will reboot and after a second or so, it will reconnect as `CIRCUITPY`.

- <strong style="color: #388e3c;">4.</strong> Now we need to install the necessary libraries on our device: Download `adafruit-circuitpython-bundle-9.x-mpy-20240730.zip` from [here](https://circuitpython.org/libraries) and extract this file to a folder.

![image](https://github.com/user-attachments/assets/2a9de41d-40e0-409e-ad0b-670d351a0293)

Navigate to lib in the recently extracted folder and copy `adafruit_hid` to the lib folder on your Raspberry Pi Pico.

- <strong style="color: #388e3c;">5.</strong> We need to create the `python` code that we want our card to run every time it starts, in `CircutlPython` the file name should be `code.py` (`main.py` in MicroPython) and save it inside our card. You can review and download the code.py file I used [here](https://github.com/embeddedJedi/BadUSB_MahirKart/blob/main/code.py) (This code is used to execute a file called `payload.dd`. And in this way it will be able to perform the commands we want in the `payload.dd` file)

<strong style="color: #388e3c;">Note:</strong> If your keyboard is not UK, you can select a language that matches your keyboard language [here](https://github.com/Neradoc/Circuitpython_Keyboard_Layouts/releases/tag/20231122) and install it on your card.

- <strong style="color: #388e3c;">6.</strong> Find a `payload.dd` script or you can do it yourself. (It is very simple to make, you just need to set the right timing and the right key presses for what I want to do. You can find the sample `payload.dd` file we used in this project [here](https://github.com/embeddedJedi/BadUSB_MahirKart/blob/main/payload.dd))

---

# Instagram Video

<a href="https://www.instagram.com/reel/CxvdougIH8q/">
    <img src="https://github.com/user-attachments/assets/a24b8ae9-c9e7-47af-ab6b-435e268e2032" alt="Instagram Video" style="width:10%; height:10%;">
</a> 


<sup>(Click here to go to the video)</sup>

---

# Resource

[Mahir Kart](https://mahirkart.net/)

[CircuitPython](https://circuitpython.org/)

[Pico-Ducky](https://github.com/dbisu/pico-ducky)

[MicroPython](https://micropython.org/)

---
