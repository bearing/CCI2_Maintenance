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

### Part 1: Setup and Line Evacuation

The first part of the procedure is concerned with setting up the turbopump and
verifying that suitable levels of vacuum can be attained with the equipment.
**The cryostat is to remained sealed for this procedure**.
Only continue on to the pumping down of the cryostat once you are convinced 
that the vacuum pulled on the hose by the turbopump is of a satisfactory level
(< 1e-7 mbar) and stable (i.e. is not perturbed if the hose or Y-adapter is
lightly jostled).

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
 17. Assuming the last step went according to plan and a pressure of 1e-3 mbar
     was reached in the first 30 seconds or so of the pump being activated,
     continue to monitor the pressure.
     A pressure of 1e-5 mbar should be easily achievable in a few minutes.
     Once this pressure has been achieved, you can safely leave the system to
     continue pumping down (note that the valve to the cryostat is 
     still closed, so you are only evacuating the pump/hose).
 18. Check the system a few times every hour or two to ensure that the 
     pressure is still steadily decreasing.
 19. A pressure of ~1e-7 mbar should easily be achievable within 24 hours.
     Once this pressure is achieved, you can move on to the next procedure -
     opening the valve to the cryostat.
     - Note: if the measured pressure does not decrease below 1e-6 mbar, 
       after 24 hours of pumping, it is recommended that you deactivate the
       pump and check the connections.
       Consider re-greasing the O-rings and restart the procedure from step 12.

### Part 2: Cryostat Pumpdown

Once a suitable and stable vacuum has been attained from the above procedure,
the valve to the cryostat can be opened.
This valve is opened by means of the plunger on the Y-adapter.

 1. Ensure that the system is ready for the cryostat should be opened.
    The pressure should be < 1e-7 mbar, the turbopump speed should be 1500 Hz,
    and the pressure should not change if the vacuum hose is gently bumped or
    wiggled.
 2. Push the plunger on the Y-adapter in towards the cryostat.
    - N.B. The pressure will increase as this part is moved; however, if the
      pressure jumps significantly (i.e. from 1e-7 mbar to 1e-4 mbar or higher)
      or the speed of the turbopump decreases from 1500 Hz, this indicates a
      breach in the vacuum line.
      Deactivate the pump using the digital on/off switch and repeat Part 1 
      from step 12 onward.
 3. Once the plunger can no longer be pushed further in, begin slowly twisting
    the plunger clockwise as you push in. The plunger will move a bit further
    in as the plunger engages with the locking mechanism on the cryostat 
    valve.
 4. Continue turning the plunger clockwise until it resists being turned
    further. This is an indication that the locking mechanism is engaged.
 5. Once the plunger has been successfully mated (locked) with the cryostat
    valve, you can open the valve to the cryostat by twisting the plunger
    counter-clockwise. Do this slowly and monitor the digital pressure gauge
    on the pump as you do so.
    - When the valve is opened, the pressure will likely increase, potentially
      to as high as 1e-5 mbar depending on how much the vacuum in the cryostat
      has degraded.
    - **If the pressure jumps to >1e-3 mbar, or the turbopump speed suddenly
        decreaes, immediately close the valve by turning the plunger
        clockwise**. Such behavior would indicate that vacuum has been lost in
        the CCI-2 cryostat. If this happens, contact your advisor before
        continuing. It is safe to leave the pump running as long as the valve
        to the cryostat is closed.
 6. Assuming everything went okay with the last step, pull the plunger away 
    from the cryostat to ensure that the valve is completely open.
 7. At this point, the cryostat is open and being "pumped down". Monitor the
    system at least once a day.
    - The pressure as indicated by the digital gauge on the pump should 
      decrease, though much more slowly.
    - A pressure of 1e-7 mbar is usually acheivable for the system. Depending
      on the starting point of the cryostat vacuum, it may take as little as
      24 hours or as long as two weeks to reach this level.
    - The valve can be closed whenever a "suitable" pressure has been 
      achieved. I typically pump down to about 1e-7 mbar which usually also
      corresponds to a minimum cryostat temperature in the range from 90-91K
      (assuming the detector is cold at the time of the pumping).

### Part 3: Ending the Pumpdown

The procedure for ending the pumpdown and returning CCI-2 to full working order
is essentially running the above two procedures in reverse.

 1. Close the cryostat valve. Push the plunger in towards the cryostat until
    it can no longer be simply pushed. Twist the plunger clockwise until the
    valve is fully closed (i.e. the plunger resists further twisting).
 2. The valve should be firmly closed; completely finger tight.
 3. Once the valve is fully closed, the plunger is disengaged from the valve
    by pulling outwards on the plunger while *very slightly* turning
    counter-clockwise. The slight counter-clockwise turn will disengage the 
    locking mechanism, but be sure you don't accidentally re-open the valve!
    If you are unsure, repeat steps 1 and 2.
 4. Once you are confident that the valve is close and the plunger has been
    disengaged, deactivate the pump using the digital on/off switch.
 5. Watch the temperature gauge on the CCI-2 cart. If the temperature rises
    drastically as the pump deactivates, the valve was not sufficiently closed.
    If the temperature rise is slow (O(1K/sec)) you can try to recover by
    immediately re-activating the pump.
    If the temperature rise is significantly faster, then vacuum has been lost.
    Contact your advisor.
 6. Wait for the pressure gauge on the pump to read ">1e3 mbar" indicating the
    line is at atmospheric pressure.
 7. **Make sure you are wearing gloves**.
 8. Start disassembling the vacuum setup by removing the clamp holding the
    vacuum hose to the Y-adapter.
    - N.B. Be ready to catch the O-ring that will fall out after the clamp has 
      been fully removed.
 9. Either cap the hose with a stopper using the same O-ring and clamp 
    (preferred) or cap the hose with a plastic stopper and store the O-ring in
    a piece of ultra high vacuum foil.
 10. 
