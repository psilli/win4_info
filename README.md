
<a name="readme-top"></a>
<div align="center"><h1><b>GPD WIN 4</b></h1>
<img src="images/BlondDentalAnchovy-mobile.gif" alt="Logo" width="600" height="400">
</div>

<!-- TABLE OF CONTENTS -->

</BR>

<div align="center"><h3>

My collection of resources such as guides, recommendations, and troubleshooting, and general information pertaining to the GPD Win 4. (Forked from lertsoft due to bad formatting, grammatical errors, and lack of cohesion in some areas. Credit to him for the template.)

</br>

<b>DISCLAIMER:</b> You are <u>COMPLETELY</u> responsible for what you do with your device. This is only a guide and you should only do that which you feel comfortable with. I nor anyone else is reponsible for anything you do with your unit.
</h3></div>

</BR>
</BR>
</BR>

# Table of Contents
<ol>
  <li>
    <a href="#getting-started">Getting Started</a>
    <ul>
      <li><a href="#test-the-hardware">Testing & Inspection</a></li>
      <li><a href="#os-installation">OS Installation</a></li>
      <li><a href="#useful-information">Useful information</a></li>
    </ul>
  </li>
  <li>
    <a href="#drivers--applications">Drivers & Applications</a>
    <ul>
      <li><a href="#official-drivers">Drivers</a></li>
      <li><a href="#screen-color-correction">Screen Color Correction</a></li>
      <li><a href="#tdp-tools">TDP Tools</a></li>
    </ul>
  </li>
  <li><a href="#tutorials">Tutorials</a></li>
  <li><a href="#accesories--parts">Accesories & Parts</a></li>
  <li><a href="#issues--troubleshooting">Troubleshooting</a></li>
  <li><a href="#specs">Specs</a></li>
</ol>

</br>

---

<!-- GETTING STARTED -->
## Getting Started:

</br>

### Testing and inspecting the device:

</br>

+ Check first for any physical abnormalities such as:
  - Serious breaks in the seams between the top shell and bottom shell
  - Gaps between the screen and the screen holder
    - According to [GPD](https://www.indiegogo.com/projects/gpd-win-4-smallest-6800u-handheld-console#/updates/22), 0.1~0.3mm variation is acceptable
  - Uneven L1/R1 bumpers
  - Abnormally-feeling/sounding triggers
  - Rear button functionaility (if they click when pressed)
  - Alignment of top USB A port
  - If all screws are present (aside from the two hidden under the bottom plastic plate)

</br>

+ Check and note BIOS version (for later) by holding the DEL key during before powering on

</br>

+ After loading into Windows, use software such as listed below to stress test the GPU and CPU and look for problems such as screen display failure or poor processing speeds.
    - [GPU - Furmark](https://geeks3d.com/furmark/)
    - [CPU - GIMPS](https://www.mersenne.org/download/)
    - Alternatively, use whatever stress-testing/benchmarking software you prefer

</br>

+ [Test all keyboard keys and buttons](https://keyboard-test.space/)

</br>

+ Test USB ports 
    - USB-C 4.0 (Top) - Should charge and transmit up to 40 Gbps
    - USB A 3.2  (Top) - Should transmit up to 10 Gbps
    - USB C 3.2 (Bottom) - Should charge and transmit up to 10 Gbps
      - [Crystal Disk Mark can be used to test storage speeds on all ports (including the MicroSD slot)](https://crystalmark.info/en/software/crystaldiskmark/)

</br>

+ Test the MicroSD card slot and monitor for connection issues. This might take some time of use to notice abnormal behavior 
  - For speed testing, make sure you use UHS-I cards and not UHS-II. The Win 4 doesn't utilize the second row of pins on UHS-II cards. For reference: 
    - <details>
        <summary>UHS-I Pin Layout</summary>
        <img src="https://cdn.discordapp.com/attachments/950574522011119707/1086109017358745660/StorageReview-SanDisk-Extreme-microSD-1TB-Bottom.jpg"> </details>
    - <details>
        <summary>UHS-II Pin Layout</summary>
        <img src="https://cdn.discordapp.com/attachments/950574522011119707/1086109017052545105/lexar-1800x-uhs-ii-micro-sd-card-32gb-back.jpg" > </details>

</br>

+ Test the screen
    - Look for dead pixels
      - [Try this if any dead pixels persist](https://www.jscreenfix.com/fix.html)
    - [Test for frame skipping](https://www.testufo.com/frameskipping)
      - If you notice frameskipping, especially at 60 fps, refer to the troubleshooting section for more info

</br>

+ Test the touchscreen for deadzones

</br>

+ Test the small IR mousepad

</br>

+ [Test your controler sticks and buttons](https://gamepad-tester.com)

</br>
</br>

<!-- OS INSTALL -->    
## OS Installation:

(For those planning to reinstall Windows or try a different OS altogether. Not required)

</br>

+ ### **Windows 10/11:**
  - GPD ISO (Windows 11):
    - [Official GPD Windows ISO](https://gpd.hk/download)
  - Stock Windows ISO:
    - Official Microsoft images:
        - [Windows 10](https://www.microsoft.com/en-us/software-download/windows10ISO)
        - [Windows 11](https://www.microsoft.com/en-us/software-download/windows11)

</br>
  
+ ### **Linux/SteamOS:**
  - Official Valve SteamOS Recovery Image:
    - [A write-up on using the Steam Deck OS on the Win 2. Not completely applicable but will help to get a good sense of what to generally expect when running SteamOS on the Win 4](https://gist.github.com/drraccoony/8a8d0a9e3dfde9fafd3e374e418d2935#setting-expectations)
     - [Official Steam Deck OS recovery image](https://help.steampowered.com/en/faqs/view/1B71-EDF2-EB6D-2BB3)
  - ChimeraOS:
    - [About](https://chimeraos.org/about/)
    - [Download](https://chimeraos.org/download/)

</br>
</br>

<!-- INFO -->
## Useful Information:

</br>

+ [Official GPD WIN4 Manual](Manuals/GPD_WIN4_User_Mannual.pdf)

</br>

+ Changing the iGPU vRAM allocation:
  >Note: The RAM on the GPD Win 4 is shared. This means that the 16GB or 32GB of RAM on the device will go to both the CPU and GPU. This could impact performance depending on the configuration. The recommended amount of vRAM is 4GB for the 16GB RAM model and 8GB for the 32GB RAM model.

  1. Enter BIOS by holding the DEL key during (re)boot
  2. Go to "Advanced" tab
  3. Go to "CBS" tab
  4. Go to "NBIO" tab
  5. Go to "GFX Configuration"
  6. Change "UMA Frame buffer Size" to the recommended value for your unit
  7. Press ESC and go to "Save & Exit" tab
  8. Select "Save Changes and Exit" and select "Yes"

</br>

+ Though primarily known for changing TDP, MotionAssistant is also capable of:
  - Enabling and configuring gyro input
  - Custom hotkeys for many system and app functions
  - Adjusting the fan curve
  - Acting as a good first or final GUI-based option for users with little technical knowledge to reliably tweak system performance

</br>

+ Reinstalling Windows is not required to get best performance. Even if you do, the results might be neglible. Only reinstall if you know what you're doing and are willing to take the time to do so

</br>

+ Using the fingerprint scanner can be a quick way to log in after boot/wake

</br>

+ Long-pressing the IR mouse button acts a right-mouse click

</br>

+ GPD's WinControl app allows one to change/turn off the trigger lights, enable/disable rumble, and map the back buttons to keyboard keys
  - As of this writing, the back buttons can only be mapped to keys from the keyboard. Controller buttons are not possible yet

</br>
</br>

<!-- DRIVERS & APPLICATIONS -->
## Drivers & Applications:

</br>

### [Official GPD drivers and programs](https://gpd.hk/gpdwin4firmwaredriver)

</br>

### Screen color correction
  - [Files](Color_Correction)
  - [GPD color correction video](https://www.youtube.com/watch?v=-QiW4Zqy-6E)

</br>

### TDP tools:

+ Motion Assistant
  ![](https://user-images.githubusercontent.com/74781086/206900788-e8e89c61-833b-4507-871c-33496eb228d1.gif)
  - [Download](https://gpd.hk/gpdwin4firmwaredriver)
  - [Manual](Manuals/Motion_Assitant_manual.pdf)
  - [Setup video](https://www.youtube.com/watch?v=M3NNxC-BYQs)

</br>

+ ciphray's bat
  ![](https://user-images.githubusercontent.com/74781086/206900455-b058a29e-f4ae-438d-b444-5b2dcbcfa981.png)
  - CLI TDP script with many functions and tweaks
  - Located for download at the gpd_devices Discord in #autotdp
  - [Video on setup and explaining how it works](https://www.youtube.com/watch?v=ZnEQ068poY0)

</br>
</br>

<!-- TUTORIALS, REVIEWS AND VIDEOS -->

## Tutorials:

</br>

+ [How to use CrystalDiskMark to test storage and USB speed](https://www.grdian.com/resources/how-to-use-crystaldiskmark-to-test-your-storage-device)

</br>

+ [Setting up Motion Assistant on the WIN4](https://www.youtube.com/watch?v=WWkmyAxn6-E)

</br>

+ [Setting up Auto TDP tool on 6800U devices](https://www.youtube.com/watch?v=ZnEQ068poY0)

</br>

+ [Disassembly of the GPD Win 4](https://www.youtube.com/watch?v=dhbx1abJWTc)

</br>

+ [Motion Assistant setup and Gyroscope benefits](https://www.youtube.com/watch?v=M3NNxC-BYQs)

</br>

+ [IC firmware fix for screen stuttering](https://www.youtube.com/watch?v=Ovp7jrJdLAc)

</br>
</br>

<!-- ACCESORIES AND PARTS -->
## Accesories & Parts:

</br>

* Batteries from GPD AliExpress store.</br>
https://www.aliexpress.us/item/3256802595312541.html?gatewayAdapt=Pc2Msite </br>
https://www.aliexpress.us/item/3256803076020665.html?gatewayAdapt=Pc2Msite </br>

</br>

* 3D files for printing accesories: </br>
***[3D model file](https://github.com/lertsoft/GPD_WIN4/releases/tag/v0.1.1-3DModel)*** </br>
***[Shoulder Buttons - L & R](https://github.com/lertsoft/GPD_WIN4/releases/tag/v0.1.1-3DModel)*** </br>
***[Trigger Buttons](https://github.com/lertsoft/GPD_WIN4/releases/tag/v0.1.1-3DModel)*** </br>
***[Grip Case](https://github.com/lertsoft/GPD_WIN4/releases/tag/0.1.3D-Model)***

</br>
</br>

<!-- TROUBLESHOOTING -->
## Issues & Troubleshooting:

</br>

+ **USB A speeds are not as advertised**
  1. Connect a USB A to USB hub and test transfer speeds
  2. If speeds are not up to standard, check that drivers are updated and current (if applicable) 
  3. If speeds are low, verify by running a check on a Linux distro (if possible)
  4. If speeds are still low, try a BIOS reset (small pinhole on the side)
  5. If a BIOS reset doesn't fix the issue, try to open the unit and confirm if the internals are properly connected
  6. If you verified that the internals are connected and the BIOS reset didn't work, contact GPD for support and/or a replacement
    
</br>
  
+ **Touchscreen is registering inputs at different spots**

  1. [Download the current driver](https://github.com/lertsoft/GPD_WIN4/releases/tag/v5.1)
  2. Install the driver
  3. Restart the device
  - If the problem still persists, contact customer service or send a message in the Discord for further assistance

</br>

+ **Touchscreen stops detecting inputs unless device is rebooted**
  - The culprit is most likely an earlier BIOS version that has been proven to cause the touchscreen to stop functioning until a reboot is performed. Visit the official GPD driver page and follow the instructions for flashing a BIOS update that fixes this problem. Contact GPD or ask in the Discord if the problem persists after updating the BIOS

</br>

+ **You notice the screen is stuttering at regular intervals in 2D games**
  1. First verify that the game you're playing doesn't suffer from vertical sync problems that cause the game itself to sutter
      - If so, apply software fixes as needed such as turning on V-Sync in game settings or forcing it through the AMD graphics panel
      - If the problem persists across different games (especially in emulated 2D games), then it's most likely that your unit has the IC firmware problem that many users have experienced. According to GPD, the Win 4 uses a chip that converts the signal going to the display from potrait to landscape so that the OS sees the screen itself as a native landscape display (beneficial for old games that output to the screen's true orientation). However, in this case, the chip's firmware is just enough out-of-sync with the display to cause the stuttering
  2.  [Refer to this document for gathering the software and hardware for flashing the IC chip](https://docs.google.com/document/d/1KVFI7zn1XTZnpUldCw3RhRy64FLF5FaSaepIormMh0w/edit?usp=sharing)
  3. Watch a video on dissasembling the unit to learn how to open it
  4. Power off the unit and open the device
  5. Once the device is open, power on and boot to BIOS. The screen needs to be on during the flash
  6. Refer back to the document in step 2 for assembling the programmer, prepping the software, and then flashing the chip
  7. On success, power-off and reassemble the unit
  8. Boot back into the OS and run the frameskipping test. If the flash worked, you should notice frameskipping on all fps speeds
      >Some stuttering will happen on all computers, no matter what. However, upon running the frameskipping test, if you no longer notice it at regular intervals like before, then the flash was a success
  - [Additionally, Phawx has released a video tutorial on how to apply the fix as well as an explanation into the problem itself](https://www.youtube.com/watch?v=Ovp7jrJdLAc)

</br>

+ IR mousepad is not responding/working properly
  - Update or reinstall the driver
    - Contact GPD or the Discord chat if problem persists

</br>
</br>

<!-- SPECS -->
## Specs:

</br>

>(Disable dark mode if image text is hard to read)

![GPD Win4](images/GPD_Win4_Specs.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
