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
'a':      toggle power spectrum
'b':      focus on 'Normal Matter' slider
'c':      focus on 'Dark Matter' slider
'l':      focus on 'Dark Energy' slider
'i':      toggle info panel
'f':      toggle fullscreen
'1','2':  move 'Normal matter' slider left,right
'3','4':  move 'Dark matter' slider left,right
'5','6':  move 'Dark Energy' slider left,right