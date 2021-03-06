How to create an ICNS file (Apple Icon Image) for OS X apps -- a simplified reminder for myself. 
===================================================================================================

- Create a 1024 x 1024 image in Photoshop or equivalent. 

-  Resize and save the following copies of the image into a new folder named after your app name.


Filename ---------- Image Size (in pixels)
_____________________________________________________________________________________________________
(at) = @

icon_512x512(at)2x.png	1024 x 1024 <br>
icon_512x512.png	512 x 512<br>
icon_256x256(at)2x.png	512 x 512<br>
icon_256x256.png	256 x 256<br>
icon_128x128(at)2x.png	256 x 256<br>
icon_128x128.png	128 x 128<br>
icon_32x32(at)2x.png	64 x 64<br>
icon_32x32.png		32 x 32<br>
icon_16x16(at)2x.png	32 x 32<br>
icon_16x16.png		16 x 16<br>
_____________________________________________________________________________________________________

- Double check all the png's in the folder are the correct sizes. Next, rename the folder to your_app_name_here.iconset
_____________________________________________________________________________________________________

e.g. 
- FontMaker.iconset
_____________________________________________________________________________________________________
- Open up a terminal window and use the following command to convert the iconset into an ICNS 

- $ iconutil -c icns path/to/iconset
_____________________________________________________________________________________________________

e.g.
- $ iconutil -c icns ~/Desktop/FontMaker.iconset
_____________________________________________________________________________________________________

If there are not any errors, you now have a completed ICNS file. 


- Add the ICNS file to your app contents resource folder or equvilent. You may have to restart this os to see the results. 

_____________________________________________________________________________________________________
<i>To learn more about the Apple Icon Image Format check out : https://en.wikipedia.org/wiki/Apple_Icon_Image_format</i>
