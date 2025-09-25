# Rebuild Sovol SV08 to use Tapchanger and up to 6 Toolheads
Sovol SV08 modification to use up to 6 print heads using TapChanger &amp; DragonBurner

1. First I've changed the LCD from the original to the BTT HDMI5. I've used the [BTT HDMI5 enclosure](https://www.printables.com/model/946297-sovol-sv08-btt-hdmi-5-v12-enclosure-compatible). I'm not really happy with this enclosure because of not working LCD buttons and too much backlash between enclosure and the cover frame, but it very robust and do the job. Other deal with this enclosure - it doesn't holds on the SV08 enclosure. You need TPU stopper [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/display) to prevent the screen enclosure to slide up and separate from the SV08 enclosure.

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/display/TPU-stopper%201.jpg?raw=true" width="200">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/display/TPU-stopper%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/display/TPU-stopper%201.jpg?raw=true" width="200">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/display/TPU-stopper%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/display/Display%20stoper.png?raw=true" width="300">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/display/Display%20stoper.png?raw=true)
2. To connect BTT HDMI5 screen I've used original USB cable, but I've connected through [small USB hub](https://www.amazon.de/dp/B0BMXDGSGS) to one of USB type A connectors on the main board. HDMI connector on the main board is only one and it is accessible only from outside. So I've found [180° HDMI adapter](https://www.amazon.de/dp/B0C9DV6ZS) and [flat HDMI cable with 90° connector](https://www.amazon.de/dp/B07R4CPX7V). To use 180° HDMI adapter I needed to make some small cut in the SV08 enclosure.

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/HDMI/HDMI-adapter%201.jpg?raw=true" width="200">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/HDMI/HDMI-adapter%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/HDMI/HDMI-adapter%202.jpg?raw=true" width="200">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/HDMI/HDMI-adapter%202.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/HDMI/HDMI-adapter%203.jpg?raw=true" width="200">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/HDMI/HDMI-adapter%203.jpg?raw=true)
3. For the future use of up to 6 print heads the original PSU 24V 150W is not enough. I've buyed a cheaper Meanwell RSP-500-24 and made custom holders for [DIN rails](https://www.amazon.de/dp/B09VQ6KJ6H). You need about 266 mm DIN rail and following printed parts [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/psu-mount)

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%201.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%202.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%202.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%203.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%203.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%204.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%204.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%205.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%205.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/psu-mount/psu-mount%206.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/psu-mount/psu-mount%206.jpg?raw=true)
4. To organize the cables underneath I've used the voron deck support as a [cable organiser](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/panels/cable-organiser_x4.stl)

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/panels/cable-organiser.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/panels/cable-organiser.jpg?raw=true)
5. For different tasks Z-endstop, Z-calibration and XYZ multi printhead calibration I've used the Nudge sensor with 3 mm rod 55 mm long because prinhead has small moving distance behind the bed.
   * To mount the Nudge sensor and custom nozzle wiper I've made special jig to bore the mounting and Nudge rod holes [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/nudge/boring-jig.STL)
 
      [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/nudge/sensor-hole-boring-jig.jpg?raw=true" width="300">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/nudge/sensor-hole-boring-jig.jpg?raw=true)
   * I've used modified Nudge sensor body to mount it to the top surface I've added 1mm so that JST XH connector is not outradged [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/nudge/nudge/nudge_2020_sovol.STL)
 
      [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/nudge/modified-nudge-body.png?raw=true" width="300">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/nudge/modified-nudge-body.png?raw=true)
   * Nudge sensor mounted using two washers and 30mm iso 7380-1 screws, two 10mm DIN 912 screws holds other two corners of the nozzle wipper holder.
 
      [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/nudge/nudge%201.jpg?raw=true" width="300">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/nudge/nudge%201.jpg?raw=true)
   * Bambulab A1 silicone nozzle wiper (for example https://www.amazon.de/dp/B0DZWXR1WL)
 
      [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/nudge/nudge%203.jpg?raw=true" width="300">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/nudge/nudge%203.jpg?raw=true)
6. To use [Tapchanger](https://github.com/viesturz/tapchanger) I've disassembled cable harness from X-, Y- motor, camera and print head cables. To organize this cables I've used 27 chain links [10x15 cable chain](https://www.amazon.de/dp/B0991GWQ6P) and [connectors](https://makerworld.com/en/models/831830-sovol-sv08-chain-set-v2)

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/cable-chain/cable-chain%201.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/cable-chain/cable-chain%201.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/cable-chain/cable-chain%202.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/cable-chain/cable-chain%202.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/cable-chain/cable-chain%203.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/cable-chain/cable-chain%203.jpg?raw=true)
7. To use as much as possible movement distance behind the bed for using nudge sensor and nozzle wiper I've used Tapchanger [Shuttle](https://github.com/viesturz/tapchanger/blob/main/Tapchanger/STL/Shuttle/Shuttle.stl) without keeper to save additional 6mm. But usual MGN12H wagon has a 0.4 mm deeping which prevents efficient snuggle the belt between the wagon and the shuttle. I've developed MGN12H adapter, which adds only 0.4 mm additional space, but fills small deeping. It is printed with first layer height 0.2 mm and further layer 0.1 mm height, but it is also suitable to print all with 0.2 mm layer.  

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/MGN12H-deeping.png?raw=true" width="390">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/MGN12H-deeping.png?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/MGN12H-riemen-adapter.png?raw=true" width="390">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/MGN12H-riemen-adapter.png?raw=true)

   Here you can see CAD reconstruction oh the problem. This is without adapter:

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/Tapchanger-shuttle-GT2-MGN12H-deeping.png?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/Tapchanger-shuttle-GT2-MGN12H-deeping.png?raw=true)
   
   And here with adapter:

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/Tapchanger-shuttle-GT2-MGN12H-deeping-adapter.png?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/Tapchanger-shuttle-GT2-MGN12H-deeping-adapter.png?raw=true)
8. I was inspired by the videos from [chilicoke](https://www.youtube.com/@chilicoke) channel [3D Printer Nozzle Cam V2](https://www.youtube.com/watch?v=DgfCFKKtKLw) and modified my Voron 2.4 to use nozzle camera. I've found very good [5MP endoscope camera](https://www.aliexpress.com/item/1005007714189699.html) with auto-focus. It allows to focus from about 18 mm distance. I use variant with 2m with soft cable. But I'll use tapchanger, and therefore I've modified shuttle to use this camera [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/tapchanger/TapChanger-Rods-12-round-sovol.STL). Modified shuttle has also mount-point for camera cable holder [STL](https://github.com/dgo42/sv08-tapchanger/tree/main/stls/tapchanger/camera-cable-toolchanger-holder) and stopper which reduces shuttle movement on the X-axe, to avoid camera tail to crash into gantry plastic parts. But the stopper allows to use entire bed - movement on the X/axe is about 358 mm. To avoid camera tail crash into X/Y motor as X-axe is on the maximal Y coordinate I've used side cuter to gently cut groove in the camera enclosure tail to route cable to the side. On the following photos you can see how to modify camera enclosure and route the camera cable:

   Camera enclosure should have cut out so, that cable may be bent and not protrude beyond the edge of the camera enclosure:

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/nozzle-camera%201.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/nozzle-camera%201.jpg?raw=true)

   Camera should be first pushed through the hole in camera cable holder underneath of the belts and cable should be tied on multiple places with cable ties. I've used 2.4mm width:

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/nozzle-camera%202.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/nozzle-camera%202.jpg?raw=true)
   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/nozzle-camera%203.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/nozzle-camera%203.jpg?raw=true)

   I've mounted other side of the camera cable using cable chain connector instead of print head cable. Print head cable will be organised using umbilical mount in the "hat". To prevent the cable from falling and to keep it in the shape of an arch I use suggested for tapchanger watch mainspring with section about 1mm<sup>2</sup> such as 0.3x3mm [Flat Spiral Coil](https://www.aliexpress.com/item/1005006731615186.html) tied with the cable using cable ties:

   [<img src="https://github.com/dgo42/sv08-tapchanger/blob/main/photos/tapchanger/nozzle-camera%204.jpg?raw=true" width="100">](https://github.com/dgo42/sv08-tapchanger/tree/main/photos/tapchanger/nozzle-camera%204.jpg?raw=true)
9. 