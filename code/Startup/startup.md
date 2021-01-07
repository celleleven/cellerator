
%Cellerator Startup Operations

% Get Real World Time

% Using time verify shutdown log to restart from crash

% If crash true notify technician and restart last process

% Compare shutdown log with Cellerator calendar

% If Cellerator calendar has task or calibration schedule, run setup code, and execute

% Update User log



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
