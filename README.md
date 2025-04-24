How to tram the bed of the Sovol Zero 3D printer
------------------------------------------------

The goal is to be able to rotate both left and right lead-screws freely and separately from each other.
That way you can rotate them until both blocks are pinched between bed and x gantry. Then the bed is level from left to right.

- turn off power and remove glass top and the metal bottom plate.
- tilt/turn the printer in a way you can easily reach belt and see the blocks (I just tilted and have it rest on the spool holder)


Pictures with instructions:


--------
METHOD 1
--------


A. 
- place blocks on both sides of extruder on X gantry

B. 
- you can move belt to lift bed upwards to X gantry if you want but this is how it will look after step D. below

C. 
Step 1) and 2) ONLY WHEN NEEDED!
I was able to just remove the belt from idler 3) by hand without loosening or removing any screw! Does not need much force.

1) loosen circled screws, no need to remove them
2) loosen screw (use the channel following the arrow)
   for me it was not needed to remove it but I completely loosened the screw
3) (push the idler left from 1) a bit to the left to release belt tension so that you can) remove the belt from idler 3)

D. 
- with the belt removed from idler 3) you are now able to rotate both lead-screws independently by hand until both blocks are pinched between bed and and x gantry


Finishing touches:

- put back belt around idler 3)
- (put back screw 2) if you loosened it completely from the hole)
- (tighten all screws)
- create new heightmap (http://<printer-ip>/heightmap) and verify if deviation is better 
- when happy with results put back bottom plate etc

--> now your bed should be reasonably level from left to right in parallel to the x gantry of the printer. Placing the belt back into position, the alignment could move a bit. Finer adjustments are easier using the belt-tooth-skipping method (next).


---------
METHOD 2:
---------


- using the belt-tooth-skipping technic for fine adjustments after using method above or just replacing it.
- maybe not for everyone but it is a tested and working method
- for explanation of procedure see video: https://youtu.be/GVRu_uX4PEk?si=_stUpJl4nDN17h4r
- in case of the Sovol Zero, you would do this underneath where the belt and couplers are located
-

--------
SHIMMING
--------


E.
- idea for front to back tramming by shimming (washers or printed shims) in corners where bed is mounted to z lead-screws with 2 screws in each corner
  tightening/loosening them has some effect but with the speed this printer is capable of, I would rather not have loosened screws
  --> as these are quite close together, the effect off adding the needed 0.2mm on either front or back side will result in a bigger change over-all than wanted
- I tested with the lowest heights you could possibly print and tried these on the lowest side (back-side for me).
  But with a difference of let's say -0.2mm in your heightmap front to back, adding 0.2mm on both back left and right sides (under the screws in picture E.) the result is     bigger than you need.
- tested also by putting shims of 0.2mm under front screws and 0.3mm under back screws (so effectively 0.1mm added to back), the results were not what I hoped for.

F.
- upon further testing, shimming using Kapton tape will get you there. Very thin, heat resistant and therefor best option to get an even bed front to back.

--> after adding several layers of Kapton tape in the lowest corner, I ended up with a 0.102mm deviation heightmap (cold) and 0.099mm hot (20m soak @100C). See 'cold after tramming.jpg' and 'hot after tramming.jpg' for heightmap results after tramming.
Not sure why the z=0 point is almost 0.3mm lower when hot, I homed the printer after soak and before the new heightmap scan. Maybe because I did alter the tightness of screw with nylock nut which holds the strain gauge underneath left front corner.

G.
- Now the latest 1.4.2 firmware moves to using eddy sensor for z offset, maybe shimming the bed itself could be done without worrying about the pressure gauge underneath      the bed.


tbc
  
