Python control for Leviton Decora Bluetooth switches
====================================================

A simple Python API for controlling [Leviton Decora switches](http://www.leviton.com/OA_HTML/SectionDisplay.jsp?section=76089&minisite=10251). This code makes use of the PyBT2 branch of Mike Ryan's [PyBT](http://github.com/mikeryan/PyBT)

Example use
-----------

This will connect and turn on the light
```
import decora

switch = decora.decora("00:21:4d:00:00:01")
switch.connect()
switch.on()
```

This will set the light to 50% intensity
```
switch.set_brightness(50)
```

And turn the lights off
```
switch.off()
```