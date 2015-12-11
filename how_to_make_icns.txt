How to create ICNS icon for OS X apps
============================================

1. Create the icon in a photoshop or equivalent at 1024 x1024 pixels. 

2. Resize and save the following copies of the image into a folder. 



Filename			Image Size (in pixels)
icon_512x512@2x.png	1024 x 1024
icon_512x512.png	512 x 512
icon_256x256@2x.png	512 x 512
icon_256x256.png	256 x 256
icon_128x128@2x.png	256 x 256
icon_128x128.png	128 x 128
icon_32x32@2x.png	64 x 64
icon_32x32.png		32 x 32
icon_16x16@2x.png	32 x 32
icon_16x16.png		16 x 16


3. Double check all the png's in the folder are the correct sizes. Next rename the folder whateveryouwanthere.iconset


4. Open up a terminal window and use the following command to convert the iconset into an icns 

$  iconutil -c icns path/to/iconset

e.g.
$  iconutil -c icns ~/Desktop/how_to_create_icns/expense_report_icon_set.iconset


5, Add the icns file to your app contents resource folder or equvilent.