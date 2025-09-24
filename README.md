# Rebuild Sovol SV08 to use Tapchanger and up to 6 Toolheads
Sovol SV08 modification to use up to 6 print heads using TapChanger &amp; DragonBurner

1. First I've changed the LCD from the original to the BTT HDMI5. I've used the [BTT HDMI5 enclosure](https://www.printables.com/model/946297-sovol-sv08-btt-hdmi-5-v12-enclosure-compatible). I'm not really happy with this enclosure because of not working LCD buttons and too much backlash between enclosure and the cover frame, but it very robust and do the job. Other deal with this enclosure - it doesn't holds on the SV08 enclosure. You need some TPU stopper (image, STL) to prevent the screen enclosure to slide up and separate from the SV08 enclosure. 
2. To connect BTT HDMI5 screen I've used original USB cable, but I've connected through [small USB hub](https://www.amazon.de/dp/B0BMXDGSGS) to one of USB type A connectors on the main board. HDMI connector on the main board is only one and it is accessible only from outside. So I've found 180° HDMI adapter (https://www.amazon.de/dp/B0C9DV6ZS) and flat HDMI cable with 90° connector. To use 180° HDMI adapter I needed to make some small cut in the SV08 enclosure (image)
3. For the future use of up to 6 print heads the original PSU 24V 150W is not enough. I've buyed a cheaper Meanwell RSP-500-24 and made custom holders for [DIN rails](https://www.amazon.de/dp/B09VQ6KJ6H). You need about 266 mm [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/psu-mount)

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%201.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%202.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%202.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%203.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%203.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%204.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%204.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%205.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%205.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%206.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%206.jpg?raw=true)
4. To organize the cables underneath I've used the voron deck support as a cable holder (image, STL)
5. For different tasks Z-endstop, Z-calibration and XYZ multi printhead calibration I've used the Nudge sensor with 3mm rod because prinhead has small moving distance behind the bed.
   * To mount the Nudge sensor and custom nozzle wiper I've made special jig to bore the mounting and Nudge rod holes (image, STL)
   * I've used modified Nudge sensor body to mount it to the top surface I've added 1mm so that JST XH connector is not outradged (image, STL)
   * Nudge sensor mounted using two 25mm DIN 912 bolts, two 10mm DIN 912 bolds holds other two corners of the nozzle wipper holder. (image)
   * Bambulab A1 silicone nozzle wiper (for example https://www.amazon.de/dp/B0DZWXR1WL)
6. To use Tapchanger (https://github.com/viesturz/tapchanger) I've disassebled cable harness from X-, Y- motor, camera and print head cables. To organize this cables I've used 27 chain links 10x15 cable chain (https://www.amazon.de/dp/B0991GWQ6P) and connectors (https://makerworld.com/en/models/831830-sovol-sv08-chain-set-v2) (image, STL)
7. 
