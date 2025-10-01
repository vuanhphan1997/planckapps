planckapps
==========

Web apps for Planck-related stuff

Simulator
---------
An HTML/Javascript simulator of the CMB power spectrum and map
allowing the user to change the values of normal matter, dark matter and dark energy

Requires:
 - A reasonably modern browser
 - To run locally, ensure browser can access local files
   - e.g. for Chrome, set flag --allow-file-access-from-files
   - the same flag works out of the box for Chromium
     when launching it from a terminal
   - while there are reocmmended steps to follow to enable local files
     in firefox, they didn't work for us, so we recommend just using Chrome/Chromium

Written by Stuart Lowe & Chris North. Modified by Anh Vu Phan

**Link**: Visit the webapp at [https://vuanhphan1997.github.io/planckapps/Simulator/](https://vuanhphan1997.github.io/planckapps/Simulator/)

CMB Widget
----------
A python GUI app to play with Fourier scales in a range of images.
Requires:
 - Python
 - numpy
 - matplotlib
 - pyfits (or astropy)
 - wxPython

Written by Bob Watson

Keyboard shortcuts
------------------
 - 'a':                 toggle power spectrum
 - 'b':                 focus on 'Normal Matter' slider
 - 'c':                 focus on 'Dark Matter' slider
 - 'l':                 focus on 'Dark Energy' slider
 - 'i':                 toggle info panel
 - 'f':                 toggle fullscreen
 - '1','2':             move 'Normal matter' slider left,right
 - '3','4':             move 'Dark matter' slider left,right
 - '5','6':             move 'Dark Energy' slider left,right
 - 'u','d':             move up/down between sliders
 - 'Left', 'Right':     move current slider left,right
 - 's':                 start (randomly generate the unverse)
 - 'r':                 restart current game
 - 'n':                 normal matter only
 - 'k':                 flatten
 - 'x':                 close "Win" screen after it appears

Suggested hardware
------------------

* At the Nikhef Science Day 2024, we used a "Rii GP100 SNES Retro USB Super Nintendo Controller"
  (amazon link [https://www.amazon.nl/Rii-Nintendo-Controller-Raspberry-Windows/dp/B073Z9MKKH/])
  to let people interact with the display.
* Two of these game controllers (see picture at `Hardware/snes_usb_controller.jpg`)
  are stored at the Nikhef Communications department.
* We recommend interfacing them using the `antimicro` tool.
  - Ubuntu, in Canonical's Universe component: https://launchpad.net/ubuntu/focal/+package/antimicro)
  - Windows: https://apps.microsoft.com/detail/9n1fcfq6p5lw?hl=en-us&gl=DE
* Based on our experience, `antimicro` will recognize the controllers
  right away after plugging them in.
* Load the config file at `Hardware/gamepad_config_cmb_display.joystick`
  for a readymade setup that maps controller buttons to the shortcuts above.

The final controller commands will be as follows:

- Up/Down on gamepad:   move up/down between sliders
- Left/Right buttons (at the back of the controller):    move current slider left,right
- Start:                start (randomly generate the unverse)
- A (red):              normal matter only
- B (yellow):           flatten
- Y (green):            restart current game
- X (blue):             close "Win" screen after it appears

If desired, the Left/Right directions of the gamepad can also be used
to toggle between sliders, but our experience is that this leads
to accidental presses of the Up/Down directions, as well.
(This may be avoided by adjusting the sensitivity thresholds in `antimicro`,
but we haven't been able to find a satisfactory setting here.)
