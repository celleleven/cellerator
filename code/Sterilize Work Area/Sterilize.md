

% Start at home and move Hand to (0,0,0)
G28 ; home all axes (X, Y, and Z)

%%%%% Scan enclosure hand tools, bench tools, and consumables
% Get Cellerator Size Variable
% Move hand to z=500
% Build Photo mosaic

% for photo cellerator x y area / camera x y area = number of images

% Move x + 1 photo width

% Move y + 1 photo width

% Date pictures and save with picture ### file name

% Scan image for QR Code

% Update QR Code data to global variables compare with last value and add to notes

% Verify QR Code volume, location, with optical distance camera calculation

% Repeat y + 1 photo width until cellerator width

% Move x + 1 loop until cellerator length

% Stitch picture mosaic

%%% Sterilize Build volume

% Build z-axis matrix with global_variables
% topographical_Matrix = 500X500

% Cycle through Tools

% Get tool (x y z) location

% get tool volume

% add z axis to matrix

% Make UV snake path plus include light distance

% Get gV_hand_tool_UV_want volume

% What is the UV light distance for sterilization???

% Move to (0,0,0)

% for cellerator x y area / UV_light x y area = number of cells

% Move z to corisponding cell on topographical_Matrix

%Move x + 1 uv_light width

% Move y + 1 photo width

% Turn on UV_Wand for determined amount of time... 30,000 J/cm2 (1 W= 1 J/sec) (www.uvp.com/pdf/ab-115.pdf)

% Verify gV_hand_tool_UV_want is on

% Repeat y + 1 UV_Wand width until cellerator width

% Move x + 1 UV_Wand length loop until cellerator length
