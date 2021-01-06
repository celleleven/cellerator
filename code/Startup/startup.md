
Cellerator Startup Operations

The user goes to the cellerator and turns it on.
Operating system starts up Cellerator software
Get real world time
Look at calendar to catch any crashes
If not crash and no calendar event
This causes the Cellerator to calibrate.
Run Calibration script  Cellerator_Startup.py
Calibrate Hand
G28; XYZ (0, 0, 0)
Calibrate Eye
; Take Picture of floor calibration sticker
; Take Picture of left wall calibration sticker
; Take Picture of the right wall. NO STICKER
; Run function that takes known value to calibrate the distances of the pictures
; Save picture with distance, meta data
; Compare calibration images with build calibration images
Scan Bench Tools
G1 Z0 F300; Move hand to top of build volume
G90; use absolute positioning for the XYZ axes
G21; metric units
G1 F3000; Move feed rate 3000
G1  X50 Y400; move to top
G4 P0; pause zero milliseconds
G1 F200; Move feed rate 200
G1  X50 Y25
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X150 Y25
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X150 Y400
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X250 Y400
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X250 Y25
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X350 Y25
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G1  X350 Y400
kCode ### Takes the picture++, Get QR Code,Save Data to global variable
G4 P0; pause zero milliseconds
G1 F3000; Move feed rate 3000
G1 X0 Y0; Move Home
; Build topographical tile scan of build volume
; plot in 3D environment ??? Does it need to be generated
Scan Hand Tools
G1 X Y Z ; Move Hand in front of hand tool 001
; Take pictures
; get QR Code data
; save data to global variable
; plot in 3D environment
Build 3D Environment
;Draw cube for build volume
;Draw cubes for bench tools
;Draw access ports for bench tools
;Label bench tools
;Draw cubes for hand tools
;Draw access ports for hand tools
;Label hand tools
Turn on LED
LED(On, RGB = 255,255,255); white light
Turn on Fume Hood. Fume hood is circulated.
If door closed
FumeHood(On, RPM = ???, time = 3 minutes)
Record air flow meter sensor data
Compare air flow meter with
Record filter exposure time
Else
Alert user
The UV wand is attached and
G1 X0, Y25, Z F300; Move to UV Wand Hand tool position 001, global variables
G1 Z??? F???; Dock to Wand
G1 X??? F???; Remove from Dock
Function test wand
; Turn on UV Light
; Is UV Light On
; Verify with picture
; Turn off UV Light
; If pass NEXT if fail alert user
Environment is sterilized
; From the 3D environment build UV sterilization path with exposure time.
NOTE: Should the entire volume be sterilized or just access ports?
Loop through x axis
Loop through y axis
If axis contains access port
Move wand to location
Turn on wand for 10 seconds
Verify with camera
Update bulb lifetime counter
Turn off wand
Next
Next
If end of loop
Park wand back and home.
Documents light bulb usage
Water line is flushed.
Move hand to waste container
Turn on water 5 seconds
Record output and compare
Turn off water
Air line is flushed
Turn on air 5 seconds
Record flow rate and compare
Turn off air.
Hand tool and bench tool functions are downloaded with any updates.
; lookup software version online
; if out dated download new code snippets
Notify user of updates.
Hand tool function test calendar, update, and
    if handbooks is new from last run function test, , should tool test only be conducted if tool it going to be used?  No





And verifies the function.


The software is launched.
The user logs into Cellerator software.


The user asks a question, and research is propagated to answer the question.


The user designs a question.
The user designs an experiment.
The user publishes the experiment for communal review and constructive feedback.
The designed experiment is converted into kCode.


The user runs the experiment
The experiment times are mapped onto the calendar, and parks steps in logical location appointment slots



Yeast transformation https://capricorn.bc.edu//bi204/wp-content/uploads/2015/08/Chapter-12-2015.pdf


Prepare a transformation master mix.  The following ingredients provide enough reagents for five transformation reactions.  Combine and mix in a microcentrifuge tube:

100 µL sterile 2 M lithium acetate (freshly prepared)
400 µL sterile 50% PEG-335
4  µL 2-mercaptoethanol (STINKY!!  add this in the fume hood!)


Add 15 µL of the denatured salmon sperm DNA (2 mg/mL) to a new microcentrifuge tube labeled with the name (or code) of the plasmid.

Note:  It is important for the salmon sperm DNA to be single-stranded for this procedure to work well.  Boil the DNA for 5 minutes to denature the DNA.  Quick chill the DNA by  placing it immediately on ice.  Keep the DNA on ice until you are ready to use it.

3. Add 5 µL of miniprep plasmid DNA to the appropriately labeled microcentrifuge tube.  4.  Add 100 µL of transformation mix from step 1 to each microcentrifuge tube.  Vortex for 10-15 seconds to mix the contents. 5.   Using a sterile toothpick or micropipette tip, scrape a large yeast colony (or the equivalent of a “match head” of yeast) from a YPD plate.  Transfer the yeast to the microcentrifuge tube containing the transformation/DNA solution (step 4) by twirling the toothpick several times.  Be sure that the cells are uniformly suspended before proceeding.
