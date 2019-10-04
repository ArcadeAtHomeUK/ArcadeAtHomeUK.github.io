# Welcome to Arcade At Home UK

To add the scanlines to carousel and menu:
Choose .png matching your raspberry pi output resolution
Rename .png with scanlines you like to scanlines.png.
Place scanlines.png image in jour theme _art folder
Modify theme.xml in theme folder (some themes use additional file, for example comic_book.xml):
In carousel section (just after </carousel>)add text

<image name="scanlines" extra="trye"> <!-- Scanlines in the Carousel (picture from _art folder) -->
<path>./_art/scanlines.png</path>
<origin>0 0</origin>
<pos>0 0</pos>
<zIndex>200</zIndex>
</image>

at the very bottom (just before </view> </feature> </theme>) add text

<image name="scanlines_2" extra="trye"> <!-- Scanlines (picture from _art folder) -->
<path>./_art/scanlines.png</path>
<origin>0 0</origin>
<pos>0 0</pos>
<zIndex>200</zIndex>
</image>

Restart emulationstation.

In MAIN MENU -> UI SETTINGS ->TRANSITION STYLE choose INSTANT mode.

If your theme support video previews, in MAIN MENU -> OTHER SETTINGS -> USE OMX PLAYER (HW ACCELERATED) -> OFF

Please note that this scanlines may significantly affect the brightness, I would recommend to choose files with 50% transparency for most old 4:3 monitors with low brightness.
