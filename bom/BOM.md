# shieldXL

## Requirements 
* [Raspberry Pi](https://www.raspberrypi.com/) - 3B, 3B+, 4B are supported. With the Pi 4B, the amount of RAM does not help/improve the norns experience. 1GB or 2GB models are great for this project  
* microSD card - use a high quality brand such as SanDisk Class 10  
* Power supply - Monome suggests using the official power supply for your model of Raspberry Pi. The Pi3B has a micro-USB power port and requires at least 2A and 5.25V ideally supplied through a cable with 24AWG or less. The Pi4 has a USB-C power port and 3A / 5.1V is recommended. Lower AWG = lower noise & more stable voltage delivery for better performance. Most consumer USB cables do not meet this spec, so please be sure to keep an eye out. You can also use a portable USB battery if it’s sufficiently large  


## Parts/Components (BOM - Bill of Materials) for pre-assembled boards

If you purchase a kit from denki-oto some of these items may be included. 

[Mouser Cart](https://www.mouser.com/ProjectManager/ProjectDetail.aspx?AccessID=c161b7b4d2) (Does not include switches)  

| Part | QTY | MFG | Part Num | Octopart | Desc |
|--------|:--:|-----|-----|-----|-----|
|1528-1785-ND|1|Adafruit Industries|2222|https://octopart.com/2222-adafruit+industries-53880117?r=sp|GPIO Header for Raspberry Pi A+/B+ - 2x20 Female Header|
|NHD-2.7-12864WDW3-M|1|Newhaven Display|NHD-2.7-12864WDW3-M|https://octopart.com/nhd-2.7-12864wdw3-m-newhaven+display-89255061|OLED Displays & Accessories 2.7 in White OLED 128 x 64 MOLEX CONNECTOR|
|PEC11R-4015F-N0024|3|Bourns|PEC11R-4015F-N0024|https://octopart.com/pec11r-4015f-n0024-bourns-26648251|24 Pulse Incremental Mechanical Rotary Encoder w/ 6 mm Flat Shaft|
|550-20311|4|Neutrik|NRJ6HF|https://octopart.com/nrj6hf-neutrik-758943?r=sp|Jack Phone 1/4 in. Stereo|
| SEE BELOW |3|Cherry/Kailh| | |Cherry MX or Kailh Choc switches|
|15167-0358|1|Molex|15167-0358|https://octopart.com/15167-0358-molex-38752501?r=sp|Display FPC Jumper Cables FFC 1.00 - 51mm| 
|Alternate Parts|
|151670356|1|Molex|151670356|https://octopart.com/15167-0356-molex-38752500?r=sp|Display FPC Jumper Cables FFC 1.00 - 31mm. Alternative to 51mm cable, this is a little cleaner but may not be availble. |
|Alternate - Yellow Display|
|NHD-2.7-12864WDY3-M|1|Newhaven Display|NHD-2.7-12864WDY3-M|https://octopart.com/nhd-2.7-12864wdy3-m-newhaven+display-84706411?r=sp|OLED Displays & Accessories 2.7 in Yellow OLED 128 x 64 MOLEX CONNECTOR|
|Optional|
|550-1005|4|Neutrik|NRJ-NUT-B|https://octopart.com/nrj-nut-b-neutrik-141986?r=sp|PLASTIC NUT|


The Display FPC Jumper Cable specs:   
20 Conductor, 1mm pitch, Opposite Side Contacts - either 31mm or 51mm will work. The 31mm is not available at Mouser.  

 	 	 	
## Mounting Hardware/Stanoffs

(still a work in progess)  

* 3-4x 11mm F/F for pi  
* 3x 8mm M/F - top side  

Optional (if not using 3d printed case)  
* 2x 16mm F/F - bottom side  

M2.5 thread screws/standoffs are used in kits.  

Knobs are up to you.  
I like these [Re-an-p670-frac-style](https://modularaddict.com/re-an-p670-frac-style-16mm-soft-touch-knob-d-shaft)  

---
## Key switches: 

The PCB is configured to use either Cherry MX or Kailh Choc (V1) switches. If you use Choc's you may want to use the spacer PCB to raise the height of the installed switch.

### Kailh Choc

Kailh Low Profile Choc Switches  

Some sources for keycaps and switches:  
US [MKUltra](https://mkultra.click/choc-switches)  
EU [Keycapsss](https://keycapsss.com/switchestester/switches/65/kailh-low-profile-choc-switches-v1)  
AU [keebd](https://keebd.com/collections/choc-switches)  

Also from Adafruit:  
[https://www.adafruit.com/product/5113 ](https://www.adafruit.com/product/5113)   
[https://octopart.com/5113-adafruit+industries-119996176?r=sp](https://octopart.com/5113-adafruit+industries-119996176?r=sp)  

| Color	| Type	| Actuation Force	| Actuation Travel	| Total Travel |
|-----|----|:---:|:---:|:---:|
|White	|	Clicky	|	60±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Brown	|	Tactile	|	60±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Red	|	Linear	|	50±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Black	|	Linear	|	60±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Pro Red	|	Linear	|	35±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|gChoc*	|	Linear	|	20±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Robin	|	Clicky	|	57±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Silver	|	Linear	|	40±10gf	|	1.5±0.5mm	|	3.0±0.5mm |
|Pink*	|	Linear	|	20±10gf	|	1.5±0.5mm	|	3.0±0.5mm |

### MX 

Any of the Cherry MX (or MX footprint) switches will work. Red/SilentRed/Blue/Brown/Black/SpeedSilver.  
Red is linear (45g). Blue is clicky & tactile (50g). Brown is tactile (45g). Black is similar to Red but 60g actuation force. SpeedSilver (shorter key travel for gamers) are linear and __Expensive__( 45g)

Cherry MX RGB part numbers:  

| Name/Color  | Part num | Type | Actuation Force |
|-----|----|-----|----|
|SilentRed |[MX3A-L1NA](https://www.mouser.com/ProductDetail/CHERRY/MX3A-L1NA/?qs=F5EMLAvA7IA6PAS7ry3I9w%3D%3D)| linear | (45g) |
|Red	|MX1A-L1NA| linear | (45g) |
|SilentBlack |[MX3A-11NA](https://www.mouser.com/ProductDetail/CHERRY/MX3A-11NA/?qs=F5EMLAvA7ICizK1XKjfN9w%3D%3D)| linear | (60g) |
|Black	|MX1A-11NA| linear | (60g) |
|Brown	|[MX1A-G1NA](https://www.mouser.com/ProductDetail/540-MX1A-G1NA/)| tactile | (45g) |
|Blue	|MX1A-E1NA| clicky & tactile | (50g) |
|Silver	|[MX1A-51NA](https://www.mouser.com/ProductDetail/CHERRY/MX1A-51NA/?qs=F5EMLAvA7IB4ByA0zXdBkg%3D%3D)| linear | (45g) |

Reference: https://www.mouser.com/pdfDocs/cherrykeyswitches.pdf

---
## Keycaps: 

NOTE - Chocs have specific keycaps and are not compatible with MX switches.

#### Chocs keycaps

MBK profile caps are great:  
US [MKUltra](https://mkultra.click/search.php?search_query=mbk&section=product)  
EU [Keycapsss](https://keycapsss.com/keyboard-parts/keycaps/182/mbk-dye-color-choc-low-profile-keycap)  
AU [keebd](https://keebd.com/products/mbk-low-profile-keycaps)  

Work Louder - wrk-dime  
[https://worklouder.cc/shop/wrk-dime/](https://worklouder.cc/shop/wrk-dime/)  

#### MX keycaps

Any MX-compatible keycaps will work, but DSA profile caps work well for this application.

[DSA "Dolch" Keyset (Two Shot) "Windowed" Keys](https://pimpmykeyboard.com/dsa-dolch-keyset-two-shot/) (choose the __LED Kit__ option).  

[Flashquark Translucent DSA Keycaps](https://flashquark.com/product/translucent-dsa-keycaps/) (in Black, White, Clear, Blue, Red) - __50 per pack__. ($12.99-$15.99 per pack)

[Blue Hat 1U DSA Blank Printed Keycaps PBT Keycaps](https://www.amazon.com/gp/product/B07SJKMNWC) (Gray Translucent) - __37 per pack__. ($15.55 per pack and prime shipping)  
(about the same as the black ones from Flashquark above)

[Maxkeyboard Black Translucent MX Blank](https://www.maxkeyboard.com/black-translucent-cherry-mx-blank-keycap-set-for-esc-w-a-s-d-or-e-s-d-f-and-arrow-keys.html) (pack of 9). 


