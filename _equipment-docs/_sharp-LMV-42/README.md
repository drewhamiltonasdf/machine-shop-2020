# Sharp LMV-42 Milling Machine

&nbsp;
&nbsp;

### Specs:

  - 42 inch table
  - 3 Horsepower R8 Spindle
  - 3-axis Digital Read-out (DRO)
  - 3-axis powerfeed
  - Automatic collet-closer
  
### The Basics: Acceptable Materials & Safety

  - This is the nicest milling machine you will likely ever encounter. Please treat it with reverence.

  - Up to a point, you can cut almost anything on a milling machine. If your cutting tool is harder than your material, you should be able to cut through it.
    That said, it is advisable to start with softer/easier materials like Delrin, work your way up to aluminum, venture into mild steel, and maybe stainless
    or tool steel with some practice and research into proper speeds and feeds. Milling machines were designed to cut difficult materials. This mill has a
    rigid cast iron construction and 3HP spindle motor. 
  
  - "Speeds & Feeds" are the most important thing to focus on if you are having trouble with difficult materials. Slower speeds and lower feeds are really not
    necessarily going to help you. The CORRECT speeds and feeds are what are going to help you.

  - 
  
### The Basics: Speeds & Feeds

  - This ![retired machinist](http://tomstechniques.com/) put together an excellent chart for calculating the appropriate spindle speeds for different materials. This is a great starting
  point:
  
  ![alt text](https://github.com/drewhamiltonasdf/machine-shop-2020/blob/main/_equipment-docs/_sharp-LMV-42/_manuals-info-etc/Tom's Techniques- Feeds & Speeds.JPG?raw=true)   
  
Example software for 2D vector design:

  - AutoCAD
  - Illustrator
  - InkScape

You can use virtually any vector design software you like, but the laser is currently set up to plot from InkScape, a freeware vector design software. In the future we can set up to plot directly from any preferred software. 
  
Lasers cut 2D vector files. File types include DXF, SVG, Illustrator files, etc. If you have a workable file-type, there are several other requirements:

    1) All vector files must be "flattened" if they contain 3D geometry. 
    
    2) All "blocks", "groups" etc must be exploded into simple vector lines (or solid hatch regions for rastering)
    
    3) To optimize cut-time and order-of-operations, join closed polygons or "polylines"
    
    4) Linewidth must be 0.000" to 0.007" to cut as a vector. (Larger linewidths may be cuttable as a raster)
    
    5) Linetype must be "continuous" (no dashed or "unspecified" linetypes etc)
    
    5) Arrange groups of lines by color, so you can specify the order in which they cut (i.e. inside vs. outside cut lines)
    
    6) Place some geometry denoting the bed-size of the laser for your reference.
    
    7) Layout all cuts with AT LEAST 1X material-thickness spacing between cut lines to increase likelihood of success.
    
    8) Maximize [cut width : material thickness] ratio to improve likelihood of success. (1:1 or better is typical).
    
    9) Mind your units: INCHES only. You may need to scale if you screwed things up. (25.4 or 1/25.4)
    

Lasers typically cut in one of two ways: raster and vector.

When rastering, the laser will etch out a region line by line like an old dot matrix printer. It is used mostly for images, but also makes it possible to engrave "3D" features like shallow depressions. It is significantly slower than vector cutting, in which the laser follows the vector lines from beginning to end. It is best practice to explode all "blocks" and "groups" etc, but leave polygons/polylines joined. This takes some experience and is one of the most common sources of issues when first using a laser. When in doubt, refer to the list above for troubleshooting.

![alt text](https://github.com/drewhamiltonasdf/machine-shop-2020/blob/main/images/readme-images/title-cutting-raster-vector1-540x338.jpg?raw=true) 

![alt text](https://github.com/drewhamiltonasdf/machine-shop-2020/blob/main/images/readme-images/rastervector.JPG?raw=true) 


### Order of Operations:

    1) Ensure USB is plugged into the laser and the computer. Ethernet is not currently workable without a network card.
    
    2) Power the laser on. The switch is on the right of the machine on the side panel.
    
    3) Open InkScape, load vector file, and follow list above for DO's and DON'Ts pertaining to file-prep.

    3) Document Properties > Custom Size > Width: 24 inches, Height 12 inches    (Reminder: make sure the units are inches)

    4) Reminder: Make sure the lineweights are 0.001"

    5) File > Print .....     [ Select Printer "Epilog Engraver" (Not the WinX64 version) ]  ... Click Print

    6) Dashboard will come up. Change Process type to "Vector" and adjust cut settings appropriate for material

    7) Click "Print"
    
    8) If you are having issues, please do not reach out unless you have gone through "The Basics: Vector Design Files".
    Please also read through this list in order one more time. Otherwise, shoot me an email at Drew.Hamilton@nyulangone.org, 
    and I can improve this document to include whatever we're dealing with.
