# CCI-2 Pump-Down Procedure

This document describes the procedure for pumping-down the CCI-2 cryostat using
the turbopump.

## PPE

The following PPE are required for the pump-down procedure:
 - Long pants (required for 1140 access)
 - Close-toed shoes (required for 1140 access)
 - Safety goggles

Though not technically for personal protection, remember that gloves **must** 
be worn when handling vacuum components.

## Safety Hazards

There are few safety hazards specific to pumping down the detector beyond those
associated with work in 1140.
A sudden loss of vacuum, while bad for the equipment, is not likely to 
represent a threat to your safety.
Safety glasses must be worn nonetheless.

## General Considerations

As mentioned in the [README](../README.md), it is important that all of the 
components that will be under vacuum are undamaged and kept clean.
Latex/nitrile gloves should be worn at all times when handling vacuum
components.
If you end up touching your skin with your gloved hand (e.g. scratching an
itch) be sure to replace the glove before continuing to handle vacuum 
components.
Unclean vacuum components can cause major headaches as they significantly 
degrade or may even prevent vacuum from being attained, but there is often no
visible evidence of the contamination.
Metallic vacuum components can be cleaned using an ultrasonic cleaning station.
Rubber or plastic vacuum components (e.g. O-rings) should be replaced rather 
than cleaned.
[McMaster-Carr](https://www.mcmaster.com/) and 
[Kurt Lesker](https://www.lesker.com/) are two lab vendors that have a wide
array of vacuum components (O-rings, flanges, clamps, hoses, etc.)

## Procedure

 1. **Ensure that there is no bias applied to the detector**.
    If the detector is currently biased, follow the ramp-down procedure before
    continuing.
 2. Turn off preamp power supply.
    This is achieved by turning off the NIM bin on the cart.
 3. Disconnect the preamplifier power cables from the DC-side preamplifier
    boxes on CCI-2.
 4. Remove the 4 screws that hold the two signal-cable cleats to the DC-side
    preamplifier boxes.
    Store the screws somewhere out of the way where they will not be lost.
    - N.B. You will need a modified allen wrench with a short "snout" to undo
      the inner most screws.
      There should be two in the CCI-2 toolbox. 
      If you can't find them, you will need to make another - the machine shop
      can cut then end off of the wrench for you.
 5. Remove the signal cable cleats and rest them on the CCI-2 cart frame.
    Try to minimize the stress on the signal cables.
 6. **Put on gloves**
 7. Remove the protective cap from the vacuum flange on the CCI-2 cryostat.
 8. Visually inspect the O-ring on the flange.
    If it appears damaged, replace it.
 9. Bring the cart with the turbopump over to the side of the CCI-2 cart 
    nearest the cryostat vacuum port.
 10. Plug the turbopump into the cart.
     - N.B. it is advisable to power the turbopump with the uninterruptible
       power supply (UPS) on the CCI-2 cart.
       This will ensure that the pump is not damaged and vacuum not lost in the
       event of a building power failure.
 11. Power up the turbopump via the green analog switch.
     **Do not activate the turbopump at this stage (via the digital switch)!**
 12. Screw the Y-shaped vacuum adapter onto the vacuum flange of the CCI-2
     cryostat.
     Use channel-locks to ensure that the adapter is tightly mounted.
     Do not tighten too much however as this can damage the O-ring.
 13. Assuming that there is already a vacuum hose attached to the turbopump,
     attach the hose to port on the Y-shaped vacuum adapter using an O-ring and
     a vacuum clamp.
     Again, I like to use the channel-locks to ensure that the vacuum clamp is
     securely mounted.
 14. Double-check all connections: pump -> hose -> Y-adapter-> cryostat.
     Ensure that each connection has an O-ring.
 15. On the digital display on the turbopump, use the arrow-buttons to toggle
     over on the display until you reach the one that says "Actual Spd".
     The digital display should then show two data: the pressure and the 
     rotational speed of the turbopump.
     With the pump off, these two displays should read ">1e3 mbar" and "0 Hz"
     respectively.
 16. Activate the turbopump using the digital on/off switch.
     Keep a close eye on the digital display of the pump.
     The pressure should begin falling, easily reaching 1e0 mbar in the first
     10 seconds and 1e-3 mbar within 30 seconds or so.
     - **If the pressure does not reach 1e-3 mbar within a minute, or at any 
       point the pressure stops decreasing and begins to increase, you have a
       leak**. De-activate the pump via the digital switch and debug the 
       vacuum system (see [this procedure](./vacuum_debug.md)).
