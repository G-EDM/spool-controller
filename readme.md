# Work in progress - Will update the readme soon

FreeCAD file for the spool holder available via google drive:
[Spool controller FreeCAD file](https://drive.google.com/file/d/11AmHV53BxJ0Tc6LzvBvqBzhYZIWUP5-e/view?usp=drive_link)


</br>
</br>
<img width="500px;" src="./images/MKS42C-wiring-0.jpg"><img width="400px;" src="./images/spool-controller-1.jpg">
</br>
</br>


# Print tips

- Main body can be printed without supports, 100% infill, 15-20mm Brim. Use adhesive on the printbed and a dustwiper on the filament! 100% infill, no support, 0.3mm layer height, 15mm Brim

- Lever and Main Body with 0.3mm layer height all others with 0.2mm


# Postprocessing

It is a heavy duty part. I use a little blowtorch lighter to remelt the parts carefully and step by step. Until the surface starts to get shiny. Not too much at a time. The part will deform and shrink and may require some rework to fit. But this provides very strong parts.

The part to clamp down the spool is a lefthanded thread. If it doesn't fit just blowtorch the threat a little, put both parts on a 12mm rod and then screw them together. Counterclockwise to screw it in.

The wire follower has two M3 screws with a large washers to clamp down the bearings. I just heat the M3 screw up and screw them in. 

The 8mm rod should be sanded and smooth to make the follower move to the left and right without issues. Maybe will remake the follower to use a linear bearing but for now this is ok.

# The Motor

The Motor is a small Nema 17 with a Makerbase 42C v.1.1 driver. Sourcing the correct board currently is a little tricky. The boards available on Ebay and Amazon are all 1.0v which will not work. The only v1.1 versions I found are the ones that ship with the big motor. To use those boards with the small motor it requires a little magnet that ships with the motorless v1.0 boards available on Amazon. Not sure about the exact Magnet.

Sourcing the boards from Makerbase directly should be possible.

Also: The 42C ships with a little JST jumper wire to connect the board with the motor. The small Motor requires the middle wires of the JST connecter to be swapped due to a different pinout.

This is all a little much and I will work on that to maybe even provide an easy source for this part.

Use the provided firmware on an ESP32 to write the settings to the motordriver once:

https://github.com/G-EDM/SERVO42C-ESP32WROOM32-UART-FLASH-SOFTEST-CONFIG

