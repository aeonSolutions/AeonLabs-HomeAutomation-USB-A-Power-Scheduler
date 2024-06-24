[![](https://dcbadge.vercel.app/api/server/hw3j3RwfJf) ](https://discord.gg/hw3j3RwfJf)
 [![Donate](https://img.shields.io/badge/donate-$-brown.svg?style=for-the-badge)](http://paypal.me/mtpsilva)
 [![Say Thanks](https://img.shields.io/badge/Say%20Thanks-!-yellow.svg?style=for-the-badge)](https://saythanks.io/to/mtpsilva)
![](https://img.shields.io/github/last-commit/aeonSolutions/PCB-Prototyping-Catalogue?style=for-the-badge)
<a href="https://trackgit.com">
<img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/l5m5z1845s10s47cuyl5" alt="trackgit-views" />
</a>
![](https://views.whatilearened.today/views/github/aeonSolutions/PCB-Prototyping-Catalogue.svg)

<br>

[PCB-Prototyping-Catalogue](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue)  >>  [Home-Automation](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/tree/main/Home-Automation)  >>   [Distributed Power Storage](https://github.com/aeonSolutions/AeonLabs-HomeAutomation-Distributed-power_storage/tree/main)  >>   USB-A Power Scheduler

<p align="right">
 <a href="https://github-com.translate.goog/aeonSolutions/PCB-Prototyping-Catalogue/tree/main?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=en&_x_tr_pto=wapp">Change Language</a> <br>
Last update: 15-04-2024
</p>
<p align="right">
    partially sponsored by <br>
    <a href="https://www.seeedstudio.com/fusion.html">
       <img height="25" src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/seedstudio_logo.png">
    </a>
</p>


# USB-A Power Scheduler

This is a simple Power Scheduler with BLE / WIFI connectivity to turn ON or OFF a USB-A port/Plug/outlet at any given day and hour. Compatible with all major commercial vendors and also open source vendors such as Home Assistant. The innovation of this  USB Power Scheduler device is in the ability to schedule charging to specific times during the day and night according to the price of electricity change. It can be programmed using machine learning to connect to an electricity market data source and calculate the best time to schedule power according to the price variations in the electricity markets. 

<p align="center">
   <img src="https://github.com/aeonSolutions/AeonLabs-HomeAutomation-USB-A-Power-Scheduler/blob/main/media/pcb_front.jpg" width="45%">
    <img src="https://github.com/aeonSolutions/AeonLabs-HomeAutomation-USB-A-Power-Scheduler/blob/main/media/pcb_back.jpg" width="45%">
</p>

<p align="center">
<strong> <a href="https://aeonsolutions.github.io/sponsor/usb_power_schedule/">Interactive view of the PCB Layout</a> </strong> &nbsp;
  <strong> <a href="https://aeonsolutions.github.io/sponsor/usb_power_schedule/circuit_schematic.html">Interactive view of the circuit schematic</a> </strong> <br>
 <sup>Click to view the latest revision</sup>
</p>

<p align="center">
   <img src="https://github.com/aeonSolutions/AeonLabs-HomeAutomation-USB-A-Power-Scheduler/blob/main/media/LK-USB07_ALIEXPRESS.jpg" height="300px">
</p>



**revision 05-2024** <br>
In this most recent revision, I'm using the microcontroller ESP32 C3 and an extreme low power management system that makes this device consume a mere ~360nA when connected to a USB plug and in standby mode.
It also features USB-A to Serial UART connectivity on the USB-A male connector for firmware upgrades & updates, and it can also be used to probe a USB Power Delivery Network. More of these Smart Scheduler Devices connected to your home "USB Power Delivery Network", that Network will be more secure and safe from hacks and intrusion.

Plus.... <br>
scheduling of charging a device for an hour more convenient, when the electricity price is lower, for instance during late-night hours.


Made to fit a cheap plastic enclosure sold on AliExpress. See the parts list below for more information. 


###  Read all about this open hardware project on ...
<p align="center">
   <a href="https://www.hackster.io/mtpsilva/usb-a-power-scheduler-acad74">
      <img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/hackster_io.png" height="50">
   </a>
 </p>

<br>


<br />
<br />


## Parts List

- buy the [Smart PCB electronics (assembled)](https://www.tindie.com/stores/aeonlabs/) o Tindie.com
- buy the [Plastic enclosure LK-USB07](https://s.click.aliexpress.com/e/_DCx3bkj) on AliExpress

<br>


## Compatibility

<p align="center">
 <a href"https://www.apple.com/shop/accessories/all/homekit">
<img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/works_with_apple_home.png" height="50">
 </a>
<a href="https://home.google.com"> 
 <img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/works_with_google_home.png" height="50">
 </a>
<a href="https://www.home-assistant.io">  
 <img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/works_with_home_assistanr.png" height="50">
 </a>
<a href="https://csa-iot.org/all-solutions/matter/">  
 <img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/works_with_matter.png" height="50">
 </a>
<a href="https://csa-iot.org/all-solutions/matter/">  
 <img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/works_with_zigbee.jpg" height="50">
 </a>
</p>

<br>

### ![](https://github.com/aeonSolutions/AeonLabs-WIFI-BLE-RFID-NFC-Desk-Contacless-Reader-Writer/blob/main/designs/working_green.png) Status
  The Smart USB-A Scheduler is now Fully functional.
  
  <p align="center">
<img src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/testing_phase_alpha.jpg" height="300">
</p>

<br>

## OEM Firmware code
The OEM version of the firmware code can be found in the folder **firmware code**.  It has by default OTA updates, meaning this smart switch device automatically updates itself when newer updated versions are made available here.  
This code uses my own ESP32 C++ class libraries to expedite the development of code for ESP32 microcontrollers. The repository is located [here](https://github.com/aeonSolutions/aeonlabs-ESP32-C-Base-Firmware-Libraries#readme) for anyone to use.


<p align="center">
 <img height="70" src="https://raw.githubusercontent.com/Domi04151309/HomeApp/main/app/src/main/res/mipmap-xxxhdpi/ic_launcher.webp">
</p>

### Home App for Android™
HomeApp is a small and easy to use smart home app with a simple framework. The goal of this application is to make remote execution of predefined features as easy and user-friendly as possible to help you get started with smart home technology.

<p align="center">
<a href="https://f-droid.org/packages/io.github.domi04151309.home">
  <img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png"
  alt="Get it on F-Droid"
  height="80"/>
</a>
</p>

<br>

<br>

## Original KiCad Project Files
The folder "KiCad Project Files" contains the KiCad Project files, for the hardware electronics of the USB-A Smart Scheduler.  Each KiCad project is available with a [creative commons share alike non-commercial license](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.en). 

<p align="center">
  <strong> <a href="https://github.com/aeonSolutions/AeonLabs-HomeAutomation-USB-A-Power-Scheduler/tree/main/KiCad%20Project%20Files">Go to The KiCad Project Files folder</a> </strong> <br>
 <sup>available with a creative commons share alike non-commercial license/sup>
</p>

However, they're not fully complete. If you like it and are looking to use it on your projects, you can download the complete Kicad project files with a one-time donation, [click here](https://github.com/sponsors/aeonSolutions) to learn how,  and don't forget to include it in a message the name of the module/hardware electronics you need. <br> Thank you 🙏.

<br />
<br />

## Author

You can get in touch with me on my LinkedIn Profile:

#### Miguel Tomas

[![LinkedIn Link](https://img.shields.io/badge/Connect-Miguel--Tomas-blue.svg?logo=linkedin&longCache=true&style=social&label=Connect)](https://www.linkedin.com/in/migueltomas/)

<a href="https://stackexchange.com/users/18907312/miguel-silva"><img src="https://stackexchange.com/users/flair/18907312.png" width="208" height="58" alt="profile for Miguel Silva on Stack Exchange, a network of free, community-driven Q&amp;A sites" title="profile for Miguel Silva on Stack Exchange, a network of free, community-driven Q&amp;A sites" /></a>

<a href="https://app.userfeel.com/t/2f6cb1e0" target="_blank"><img src="https://app.userfeel.com/tester/737648/image?.png" width="257" class="no-b-lazy"></a>

You can also follow my GitHub Profile to stay updated about my latest projects: [![GitHub Follow](https://img.shields.io/badge/Connect-Miguel--Tomas-blue.svg?logo=Github&longCache=true&style=social&label=Follow)](https://github.com/aeonSolutions)

<br>

**Hire me** <br>
See [here](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/wiki/How-to-Hire-AeonLabs) how to hire AeonLabs.

<br>

### Be supportive of my dedication and work towards technology education and buy me a cup of coffee
The PCB design Files I provide here for anyone to use are free. If you like this Smart Device or use it, please consider buying me a cup of coffee, a slice of pizza or a book to help me study, eat and think new PCB design files.

<p align="center">
    <a href="https://www.buymeacoffee.com/migueltomas">
        <img height="35" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png">
    </a>
</p>


### Make a donation on PayPal
Make a donation on PayPal and get a TAX refund*.

<p align="center">
    <a href="http://paypal.me/mtpsilva">
        <img height="35" src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/paypal_small.png">
    </a>
</p>

### Support all these open hardware projects and become a GitHub sponsor  
Did you like any of my PCB KiCad Designs? Help and Support my open work to all by becoming a GitHub sponsor.

<p align="center">
    <a href="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/become_a_sponsor/aeonlabs-github-sponsorship-agreement.docx">
        <img height="50" src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/want_to_become_a_sponsor.png">
    </a>
    <a href="https://github.com/sponsors/aeonSolutions">
        <img height="50" src="https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/media/become_a_github_sponsor.png">
    </a>
</p>

# 

### License

Before proceeding to download any of AeonLabs software solutions for open-source development and/or PCB hardware electronics development make sure you are choosing the right license for your project. See [AeonLabs Solutions for Open Hardware & Source Development](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/wiki/AeonLabs-Solutions-for-Open-Hardware-&-Source-Development) for more information. 
