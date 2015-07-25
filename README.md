# textilo
free hardware electronic textile platform ( based on NE555 ) -- All code in GPLv2 & content in Creative Commons CC0 & CC-BY-SA 4.0.

## 10 steps to assemble a textilo soft electronic board

* 1. Locate ( https://github.com/jeanbaptiste/textilo/blob/master/README.md ) , Read in your language & Understand this tutorial :)
* 2. Order the components 
	* 5x5 cm Flectron conductive textile http://www.lessemf.com/1212.pdf (Thickness: 0.08mm (3 mil)- Weight: 80 g/m² (about 35% Copper)- Surface Resistivity: 0.05 Ohm/sq. )
	* 5 x 5 Neoprene textile
	* 5 cm fusible glue paper
	* Mild Adhesive
	* 10 uF *polarized* capacitor
	* 100 uF *polarized* capacitor
	* 100 Ohms resistance 
	* NE555 timer IC in DIP (dual inline package)
* 3. Cut a 5 cm neoprene disc (lasercut it or use a punch or scissors)
* 4. With a CNC machine (plotter, lasercutter) cut the Flectron circuit after sticking paper tape to it. Here is the source code for the cut https://github.com/jeanbaptiste/textilo/blob/master/schematics/textiloBIG.svg . Please credit accordingly, remix & share. 
* 5. Once the circuit is cut, apply mild adhesive before removing it from the machine
* 6. Remove unwanted parts of the circuit (intermediary traces) with tweezers
* 7. Place the circuit on the neoprene, remove mild adhesive and iron it
* 8. Solder the 4 components (555 IC, 100 ohms resistance, 10 & 100 microfarads capacitors) according to the schematics at the bottom of this page (available here as well https://github.com/jeanbaptiste/textilo/blob/master/schematics/textiloBIG.png  )
* 9. Test by placing a 3v to 15v battery on the PLUS & round pad underneath it, THEN a resistive sensor on the two upper pads (INPUT) and THEN an actuator (8 ohm speaker for instance) on the two lower pads (OUTPUT).
* 10. Connect any sensors and outputs, share your creations & improve world karma ^^

### schematics

<img src=schematics/textiloBIG.png width=400>

### finished textilo

<img src=/pictures/testrun.Textilo.DataPaulette.July/IMG_0860.JPG>

## How textilo works ?

### the 555 

Textilo uses a cute and popular electronic component: the 555 Integrated Circuit (IC). This amazing piece of equipment has been created in designed in 1971 by Hans Camenzind. The standard 555 package includes 25 transistors, 2 diodes and 15 resistors on a silicon chip installed in an 8-pin mini dual-in-line package (DIP-8).

Wikipedia has a great page about it: https://en.wikipedia.org/wiki/555_timer_IC

When used in 'astable' mode, the 555 IC becomes an oscillator, capable of generating a specific frequency as an output of a variable resistance place as an input.

The 555 is very tolerant in terms of voltage, it can receive from 3 to 15 volts. It outputs a maximum of 2,7 volts approximatively. This means you can directly connect low power actuators such as speakers but not an LED or a motor which will require an additional (simple) circuit. You can use a jack to plug your textilo in the soundcard of your computer, making it a very simple & cheap interface to control stuff with it!

### how to 'program' textilo

Well, textilo is not 'programmed' with software but with specific hardware configuration. It means that you do not need to input 'code' to textilo but you have to configure it by placing specific electronic components at its pins. The values of these different components will impact the way it behaves, hence "predicting" its future state. In a way, this is a kind of hardware or analogue 'programming' but with no text or code input. 

### can i create my own sensors and actuators for textilo ?

Absolutely! Check out the amazing repository of inspirations at Hannah's & Mika's fabulous website http://www.kobakant.at/DIY

### i want to share & credit other works, how can i do ?

Textilo is free hardware (GPLv2) & creative commons content (CC0, CC-BY-SA 4.0). This implies you have to credit & mention the files & examples in your future creations, presentations, workshops & classes. A simple link to this GitHub page is a good start ^ ^

Next step is *Documentation*, taking pictures of your works, creating tutorials for others and sharing the files with free licenses so that people can understand and remix them. 

Recent theories insist on how we deeply *learn by sharing* . Documentation is the way to reflectively re-organize our knowledge. Sharing puts us in the position of thinking towards how others will perceive our work, allowing a "perspective shift" which is definitely worth many points of IQ !

### do you organize events related with textilo ? 

The first textilo event happened at DataPaulette www.datapaulette.org textile hackerspace in Paris in July 2015. Textilo will then be part of the Etextile Summer Camp (Swatchbook entry) http://etextile-summercamp.org/  and Pa-F www.pa-f.net philosophy week workshop on hands-on metaphysics.


