# Humphrey2
A self replicating large format open hardware CNC router

*by Jens Dyvik, March 2022 - ongoing*

### Index

 - [Dev log]()
 - [Bill of materials]()
 - [CAD file of assembly]()
 - [Files for CNC milling]()
 - [Files for 3D printing]()
 - [License]()


### Dev log November 29th 2022 - Good test cuts and promising self-replication

![](img/humphrey2-with-test-objects.JPG)
*15mm poplar plywood cut in one pass at 4200mm/m, 50mm styrofoam 3D milled and 8mm aluminium test pattern*

![](img/humphrey2-alu-test.JPG)
*Accuracy seems to be about +- 0.1mm. 6082 Aluminium cut with a 6mm single flute bit. 0.7mm pass depth, 1440mm/m feedrate + finish pass*

![](img/humphrey2-cutsheet.png)
*All phenolic parts for a Humphrey2 fit on one 2440mm x 1220mm x12mm sheet. The same size as the work area.*

![](img/humphrey2-self-replication-test.JPG)
*Test milling of parts went well*

![](img/humphrey2-self-replication-test2.JPG)
*Cutsheet with all the leftover material removed. Note all the screws holding down each part allowing for a finish pass*



### Dev log October 31st 2022 - Smooth sailing for first test milling of parts and assembly

![](img/first-prod-and-assembly-01.JPG)
*Very few hickups during first assembly - next up lots of testing*

![](img/first-prod-and-assembly-02.JPG)
*Full size phenolic sheet loaded on [Hanzo](https://github.com/Fabricatable-Machines/Hanzo), ready to become Humphrey2 parts*

![](img/first-prod-and-assembly-03.JPG)
*It felt great to use [Hanzo](https://github.com/Fabricatable-Machines/Hanzo), a Fabricatable machine, to make another Fabricatable machine!*

![](img/first-prod-and-assembly-04.JPG)
*Using leftovers to make X - Z assembly parts*

![](img/first-prod-and-assembly-05.JPG)
*The cross pieces were also milled from leftovers*

![](img/first-prod-and-assembly-06.JPG)
*Batch milling pinions from POM plastic leftovers*

![](img/first-prod-and-assembly-07.JPG)
*The cross pieces ensure constant distance between the left and right X rail, and function as torsion box spacers*

![](img/first-prod-and-assembly-08.JPG)
*All holes thread milled during production makes assembly fast*

![](img/first-prod-and-assembly-09.JPG)
*Using a spade drill to counterbore the carriage bolt holes*

![](img/first-prod-and-assembly-10.JPG)
*The two plywood sheets that make up the top and bottom torsion box skin of the bed can be drilled manually on site. This makes for cheaper and easier shipping of the milled parts.*

![](img/first-prod-and-assembly-11.JPG)
*The adjustable feet enable leveling. What kind of sawhorse or legs to use is open.*

![](img/first-prod-and-assembly-12.JPG)
*Using masonry thread and three washers to make the outer walls carrying the X rails as straight as possible. As spirit level is used to try to make the assembly flat.*

![](img/first-prod-and-assembly-13.JPG)
*The gantry has spacer nuts so shorter screws can be used*

![](img/first-prod-and-assembly-14.JPG)
*Again, all holes thread milled during manufacturing makes assembly super fast*

![](img/first-prod-and-assembly-15.JPG)
*Gantry feet parts*

![](img/first-prod-and-assembly-16.JPG)
*Tightening under pressure*

![](img/first-prod-and-assembly-17.JPG)
*Mounting rails and racks*

![](img/first-prod-and-assembly-18.JPG)
*Mounting the X-Z carriage*

![](img/first-prod-and-assembly-19.JPG)
*Mounting gearboxes to the steppers and pinion and motor plates to the gearboxes*

![](img/first-prod-and-assembly-20.JPG)
*Gantry detail. The pinions should be snug but not too tight against the racks.*

![](img/first-prod-and-assembly-21.JPG)
*Preparing for electronics work. I am testing the OpenBuilds Blackbox and Interface for fast and easy wiring.*


### Dev log October 4th 2022 - Nesting done + design tweaks

Next up; machining, assembly and testing!

![](img/cad-process-round4-0-top-view.JPG)
*59 parts to machine from phenolic resin composite, all from a single cutsheet*

![](img/cad-process-round4-1-nested-perspective.JPG)
*Portrait of a self replicating machine*

![](img/cad-process-round4-2-z-pobe.JPG)
*Added probe plate for Z axis probing of bit length*


### Dev log September 9th 2022 - Initial design is done!

Finally the first version of the design is done. The FreeCAD model is fully parametric, which feels great. So it is possible to change parameters like material thickness, tolerances, clearance between the gantry and the bed and so on without breaking the model. Next up is test milling some parts and maybe do some parameter tuning before milling all the parts for the first prototype!

![](img/cad-process-round3-6.JPG)
*Proportions feel good*

![](img/cad-process-round3-5.JPG)
*The skeleton without the plywood torsion box skins and the sacrificial MDF layer*

![](img/cad-process-round3-4.JPG)
*Close up of the gantry and XZ axis*

![](img/cad-process-round3-0.JPG)
*Front view*

![](img/cad-process-round3-1.JPG)
*Side view*

![](img/cad-process-round3-2.JPG)
*Top view*

![](img/cad-process-round3-3.JPG)
*A rough nesting test indicates that all the milled parts will fit on one cutsheet as planned!*



### Dev log August 2022 - CAD progress and a FreeCAD bug

The master CAD design is progressing slow and steady. I ran into a bug with FreeCAD expressions *(reported [here](https://forum.freecadweb.org/viewtopic.php?f=3&t=71309&p=620375#p620375))*, so I have reverted to using FreeCAD version 19 for now. It has been nice to use the relatively new FreeCAD Link feature to make a simple assembly by embedding the external rack and pinion file. Saving both computation time and storage space :)

![](img/cad-process-round2-3.JPG)

![](img/cad-process-round2-1.JPG)

![](img/cad-process-round2-2.JPG)


### Dev log June 2022 part2 - Starting the CAD master design file

I have started making the proper design file in Freecad. The work in progress file is published and reguraly updated [here](https://github.com/Fabricatable-Machines/Humphrey2/blob/main/humphrey2.FCStd).

![](img/cad-process2.JPG)
Work in progress phenolic skeleton

![](img/cad-process1.JPG)
I am nesting the parts onto the bed of the machine as I go. The goal is to be able to cut all critical parts from one cutsheet.

![](img/cad-process3.JPG)
Plywood above and below the skeleton makes up the torsion box. The top layer is a MDF plate as a scarafical layer

![](img/cad-process6.JPG)
Test nesting onto the bed of the 3D model.

### Dev log June 2022 - Testing construction principles and components

![](img/test-piece-0-location.JPG)
In order to test design ideas, I decided to make a 1:1 test of a small cutout section of the machine bed

![](img/test-piece-1-milling-on-hanzo.JPG)
The [Hanzo](https://github.com/Fabricatable-Machines/Hanzo) machine that I developed and built is now operatoinal. It feels great to use one fabricatable machine to make the parts for the next one!

![](img/test-piece-2-cut-sheet.JPG)
Cutsheet for the phenolic resin cardboard composite test parts.

![](img/test-piece-3-birch-ply.JPG)
The plywood edges came out super clean and straight on Hanzo, using a 6mm compression cutter in two passes.

![](img/test-piece-4-assembly.JPG)
The phenolic pieces screw together with tapped holes.

![](img/test-piece-5-assembly.JPG)
Testing to use a marker to mark positions for pre drilled holes. I want avoid having to CNC machine the 2440mm x 1220mm plywood sheets.

![](img/test-piece-6-assembly.JPG)
Drilling the plywood sheets by hand will mitigate the need for shipping plywood sheets with the phenolic machine parts, instead they can be sourced locally.

![](img/test-piece-7-assembly.JPG)
100mm wood screws will lock the torsion box bed together.

![](img/test-piece-8-assembly.JPG)
The [CNC friendly](https://github.com/fellesverkstedet/fabricatable-machines/wiki/Modules#cnc-friendly-rack-and-pinion) rack screws into the side wall with quite tight tolerances.

![](img/test-piece-9-assembly.JPG)
A 15mm linear rail mounts above the rack into tapped holes.

![](img/test-piece-10-milling-pinion.JPG)
Milling a [CNC friendly](https://github.com/fellesverkstedet/fabricatable-machines/wiki/Modules#cnc-friendly-rack-and-pinion) pinion in POM on [Hanzo](https://github.com/Fabricatable-Machines/Hanzo).

![](img/test-piece-11-flexure-test.JPG)
First test assembled. I have mixed feelings about the flexure that ensure constant preload between the pinoin and the rack.

![](img/test-piece-12-motor-plate-test.JPG)
A second test with a more classic adjustable motorplate instead of flexures.

**Notes from making and testing:**

 - Tolerance for milled sides needs to be bigger.
 - Leading chamfer/fillets for slots will help in assembly.
 - Tapping though 12mm material with4 tap diffiult. Note for screw length.
 - Outer wall can be mounted upside down. Hoka poka.
 - 100mm screws are easy to get very skew.
 - A flexure at 60x4mm dimension is much too stiff. 60x2mm seems promising.
 - The flexure vibrates a bit at higher speeds.
 - Not enough space for indents in pinion that show set screw hole drill positions. 3 tabs can do the same job.
 - Cut depth of pinion teeth reduced to 5.6mm because of available 2mm bit flute lengths
 - Inside hole set to 14.05mm. Premilled to ø 13.6, then ran three times at ø14.05mm with a long 5deg ramp continuous to the bottom. Still the bottom of the hole became too small. Maybe reduce thickness of stock?
 - Motorplate with three screws instead of flexures feels safer and more suitable.
 - Openbuilds controller and interface is easy to work with.
 

### Dev log March 2022 - early sketches

![](img/humphrey2-rough-3d-sketch-with-plywood-top-and-bottom.JPG)

![](img/humphrey2-rough-3d-sketch-core-parts.JPG)

![](img/humphrey2-nesting-test-critical-parts.JPG)

### BOM
*Work in progress*

![](img/BOM-humphrey2.JPG)

### License

Creative Commons Attribution-ShareAlike
http://creativecommons.org/licenses/by-sa/4.0/
