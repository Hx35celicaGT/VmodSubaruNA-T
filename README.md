use at your own risk, it was tested on my 2006 forester ecu E2VG221D “22611AK740” label
please read through the list, special notes on flex fuel input

Patch Adds the following 
-	More sensor calibrations
-	Engine load B maximum 
-	Single ignition table (removed B-F) 
-	Switch from G/rev to Map ignition axis 
-	Over Boost fuel cut
-	Over run fuel disable for deceleration
-	Flex fuel rear 02 input
!!	If not using disconnect rear 02 from input !!
!!  Must use a 0-5V flex fuel converter
-	Launch control fuel cut rpm activation rpm
-	Launch control fuel cut activated throttle opening
-	Launch control static timing
-	Coil dwell table 
------------------------------------------------------------------------------------------
- Add “E2VG22VM” to EcuFlash “forester2.5” in the rommetadata folder
- Add “E2VG221D_Vmod” to the Romraider definition file manager
- Open up “VmodBase_01” in romraider. This file should be pretty close to stock but it may need changed for your configuration. 
- In Romraider logger add the “VmodLogger” to log all the normal parameters plus flex fuel voltage, otherwise the normal “E2VG221D” parameters will work.
- To flash use EcuFlash, if using a Vagcom or any other Obd2 connector setup and use FastEcu. 
