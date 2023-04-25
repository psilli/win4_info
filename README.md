
<a name="readme-top"></a>
<div align="center"><h1><b>GPD WIN 4</b></h1>
<img src="images/BlondDentalAnchovy-mobile.gif" alt="Logo" width="600" height="400">
</div>

<!-- TABLE OF CONTENTS -->

</BR>

<div align="center"><h3><b>DISCLAIMER:</b> You are <u>COMPLETELY</u> responsible for what you do with your device. This is only a guide and you should only do that which you feel comfortable with. I nor anyone else is reponsible for anything you do with your unit.</h3></div>

</BR>
</BR>
</BR>

# Table of Contents
<ol>
  <li>
    <a href="#getting-started">Getting Started</a>
    <ul>
      <li><a href="#test-your-hardware">Test your unit</a></li>
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
  <li><a href="#videos">Videos</a></li>
  <li><a href="#accesories--parts">Accesories & Parts</a></li>
  <li><a href="#issues--troubleshooting">Troubleshooting</a></li>
  <li><a href="#specs">Specs</a></li>
</ol>

</br>

---

<!-- GETTING STARTED -->
## Getting Started:

</br>

### Test your hardware:

</br>

+ Check for any physical abnormalities:
  - Seams between the top shell and bottom shell
  - Gaps between the screen and the screen holder
    - More than normal gaps between the sliding screen and keyboard, (According to [GPD](https://www.indiegogo.com/projects/gpd-win-4-smallest-6800u-handheld-console#/updates/22) 0.1~0.3mm variation is acceptable tolerance)
  - Triggers if they're even or uneven

</br>

+ Test the GPU and CPU under load and look for problems such as screen display failure or poor processing speeds
    - [GPU](https://geeks3d.com/furmark/)
    - [CPU](https://www.mersenne.org/download/)

</br>

+ Check BIOS version (only update if necessary)

</br>

+ [Test all keyboard keys and buttons](https://keyboard-test.space/)

</br>

+ Test USB ports 
    - USB-C 4.0 (Top) - Should charge and transmit up to 40 Gbps
    - USB A 3.2  (Top) - Should transmit up to 10 Gbps
    - USB C 3.2 (Bottom) - Should charge and transmit up to 10 Gbps
      - [Crystal Disk Mark can be used to test storage speeds on all the  ports including MicroSD slot](https://crystalmark.info/en/software/crystaldiskmark/)

</br>

+ Test the MicroSD card slot. Look for disconnecting and reconnecting issues. This issue might take a day or two of use to notice any unexpected behavior. 
  - If testing Micro SD card slot speed make sure you use UHS-I cards and not UHS-II. The GPD Win4 does not utilize the second row pins of UHS-II: 
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

</br>

+ Test the Touch screen for deadzones. (dragging your finger across the entire screen could help finding any)

</br>

+ Test the small touchpad (if it doesn't work or is not working properly try updating the firmware)

</br>

+ [Test your controler sticks and buttons](https://gamepad-tester.com)

</br>
</br>

<!-- OS INSTALL -->    
## OS Installation:

</br>

+ ### **Windows 10/11:**
  - GPD ISO (Windows 11):
    - [Official GPD Windows ISO](https://gpd.hk/download)
    - Install Windows
  - Stock Windows ISO:
    - Download one of the official Microsoft images:
        - [Windows 10](https://www.microsoft.com/en-us/software-download/windows10ISO)
        - [Windows 11](https://www.microsoft.com/en-us/software-download/windows11)
    - Install Windows

</br>
  
+ ### **Linux/SteamOS:**
  - Official Valve SteamOS Recovery Image:
     - [Official Steam Deck OS recovery image](https://help.steampowered.com/en/faqs/view/1B71-EDF2-EB6D-2BB3)
     - [A write-up of Steam Deck OS on the Win 2 that serves as a good base of what to generally expect when running SteamOS on the Win 4](https://gist.github.com/drraccoony/8a8d0a9e3dfde9fafd3e374e418d2935#setting-expectations)
  - ChimeraOS:
    - n/a

</br>
</br>

<!-- INFO -->
## Useful Information:

</br>

+ [GPD WIN4 Manual](Manuals/GPD_WIN4_User_Mannual.pdf)

</br>

+ Booting from a USB Drive
  - Hold DEL key during boot

</br>

+ [Use Custom Resolution Utility (CRU) to create different screen refresh rate ie. 40hz](https://www.monitortests.com/forum/Thread-Custom-Resolution-Utility-CRU)
  - GPD took away the option of 40hz on the WIN4 panel because of frame skipping, and stability. This tool allows you to create that refresh rate and use

</br>

+ Changing the iGPU vRAM allocation:
  >Note: The RAM on the GPD Win 4 is shared. This means that the 16GB or 32GB of RAM on the device will go to both the CPU and GPU which could hamper performance of the device depending on the configuration. The recommended amount of vRAM is 4GB for the 16GB RAM model and 8GB for the 32GB RAM model.

  1. Enter BIOS by holding the DEL key during boot
  2. Go to "Advanced" tab
  3. Go to "CBS" tab
  4. Go to "NBIO" tab
  5. Go to "GFX Configuration"
  6. Change "UMA Frame buffer Size" to desired value, the recommended value is 4GB for the 16GB RAM model, and 8GB for the 32GB RAM model.
  7. Press ESC and go to "Save & Exit" tab
  8. Select "Save Changes and Exit" and select "Yes"

</br>
</br>

<!-- DRIVERS & APPLICATIONS -->
## Drivers & Applications:

</br>

### [Official Drivers](https://gpd.hk/gpdwin4firmwaredriver)

</br>

### Screen Color Correction
  - [Files](Color_Correction)
  - [GPD color correction video](https://www.youtube.com/watch?v=-QiW4Zqy-6E)

</br>

### TDP Tools:

+ Motion Assistant
  ![](https://user-images.githubusercontent.com/74781086/206900788-e8e89c61-833b-4507-871c-33496eb228d1.gif)
  - GPD app for controlling performance, gyro, and other system settings
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

+ Power Control Panel v2
  ![](https://user-images.githubusercontent.com/74781086/206900406-57df3589-3ee1-47e6-a303-9cdc6c9552c1.png)
  - GUI for controlling TDP and other system settings
  - [Download](https://github.com/project-sbc/Power-Control-Panel-v2)

</br>

+ [Handheld Companion](https://github.com/Valkirie/HandheldCompanion/tree/0.14.0.9)

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
</br>

## Videos:

</br>

+ [In-Depth review from Notebookcheck](https://www.notebookcheck.net/GPD-Win-4-handheld-PC-review-1080p-Ryzen-7-gaming-in-the-palm-of-your-hand.700543.0.html) 
  > Note: The microSD card that they used for their test is UHS-II which can reach speeds faster than the card slot on the Win 4 is capable of

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
  
+ **Touchscreen is not working/registering inputs at different spots**

  1. [Download the current driver](https://github.com/lertsoft/GPD_WIN4/releases/tag/v5.1)
  2. Install the driver
  3. Restart the device
  - If the problem still persists, contact customer service or send a message in the Discord for further assistance

</br>
</br>

<!-- SPECS -->
## Specs:

</br>

>(Disable dark mode if image text is hard to read)

![GPD Win4](images/GPD_Win4_Specs.png)

* Comparison between the AMD 6800U and The AMD 7735 APU </br>

> (This is for future reference for those wanting to determine which APU is better)

![AMD6800U VS AMD7735](images/AMD6800U_VS_AMD7735.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
