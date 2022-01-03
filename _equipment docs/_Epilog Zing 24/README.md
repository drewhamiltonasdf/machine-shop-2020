# Epilog Zing 24 Notes

&nbsp;
&nbsp;

* #### username:     .\Laser_User
* #### password:     1qaz2WSX

&nbsp;
&nbsp;

### The Basics: Vector Design Files

Lasers cut in one of two ways: Raster / Vector
When rastering, the laser will etch out a region line by line like an old dot matrix printer. It is used mostly for images, but also makes it possible to engrave "3D" features like shallow depressions. It is significantly slower than vector cutting, in which the laser follows the vector lines from beginning to end. It is best practice to explode all "blocks" and "groups" etc, but leave polygons/polylines joined. This takes some experience and is one of the most common sources of issues when first using a laser.

* #### Sharp LMV, 49" table, collet closer, 3-axis DRO, 3-axis powerfeed, and coolant-system.

![alt text](https://github.com/drewhamiltonasdf/machine-shop-2020/blob/main/images/equipment-images/images/readme images/title-cutting-raster-vector1-540x338.jpg?raw=true) 

![alt text](https://github.com/drewhamiltonasdf/machine-shop-2020/blob/main/images/equipment-images/images/readme images/rastervector.JPG?raw=true) 

Lasers cut 2D vector files. File types include DXF, SVG, Illustrator files, etc. 

Currently we only have Inkscape on there which is a freeware vector program.




##### 1) Ensure USB is plugged into the laser and the computer. Ethernet is not currently workable without a network card.
##### 2) Power the laser on. The switch is on the right of the machine on the side panel.
##### 3) Document Properties > Custom Size > Width: 24 inches, Height 12 inches    (make sure the units are inches)
##### 4) Make sure the lineweights are 0.001"
##### 5) File > Print .....     [ Select Printer "Epilog Engraver" (Not the WinX64 version) ]  ... Click Print
##### 6) Dashboard will come up. Change Process type to "Vector" and adjust cut settings
##### 7) Click "Print"
