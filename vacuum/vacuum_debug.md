# Quick Note on Debugging Vacuum Problems

This document provides some high-level guidance for the situation where 
high-vacuum cannot be obtained with the turbopump.

## PPE

Same as all vacuum work

## Safety Hazards

See [the pumpdown procedure](./pump_down_procedure.md).

## General Considerations

The first step in "pumping down" CCI-2 is to verify that you are able to 
attain high vacuum (pressure < 1e-7 mbar) on the vacuum line itself, before
opening the cryostat.
If high vacuum cannot be pulled on the line, there is likely a leak or a
dirty component somewhere on the vacuum line.
This situation must be rectified if the cryostat is going to be pumped down.

If a pressure lower than 1e-7 mbar cannot be obtained after 24 hours of 
pumping, deactivate the pump (via the digital switch) and consider the 
following debugging steps.

As always, **make sure you are wearing gloves when handling the vacuum
components**.

Also, never attempt to disassemble a vacuum system while the pump is running
or parts of the system are under vacuum.
Deactivate the pump and wait for the gauge to indicate that the system is at
atmospheric pressure before disassembling anything.

### 1. Loose Vacuum Connections

The most likely culprit is that one of the connections is not air-tight.
Inspect the connection between the CCI-2 vacuum port and the Y-adapter.
In my experience, the Y-adapter should screwed down beyond "finger tight".
Consider using the channel-locks to tighten this connection.
Note however that the adapter should not be torqued on *too* tightly or you
risk pinching the O-ring.

The next connection to consider is the connection between the vacuum hose and
the Y-adapter.
In my experience, this too should be more than "finger-tight".
Use the channel-locks to tighten the clamp.
There is less risk of pinching the O-ring here given the nature of the
connection.

Ater tightening these two connections, activate the pump.
By the time the turbo spins up to 1500 Hz (~several minutes) you should be
able to reach pressures of less than 1e-6 mbar.
If you successfully reach this level, let it sit and check on it again in an
hour or two.
By that time you should be on the order of 1e-7 mbar.

If this didn't fix your problem, move on to the next step.

### 2. Failed/Dried-out O-Rings

In my experience, the O-rings are the next-most-likely culprit.

Ensure that the pump is deactivated and the pressure at atmospheric before
disassembling the vacuum system.
Start by disconnecting the hose from the Y-adapter, then the Y-adapter from the
cryostat.
Each of these connections has its own O-ring.
Visually inspect these O-rings to verify there is no tearing/pitting on them.
If you see some sort of irregularity, replace the O-ring.
Replacements should be in the "vacuum fittings" drawer in 1110C.

Assuming there is no visual evidence of damage to the O-rings, the next step
is to apply some high-vacuum grease.
While wearing gloves, squeeze a small amount of the vacuum grease on one of 
your fingers, and apply liberally all around the surface of the O-ring.
The entire surface of the O-ring should be "moistened", but there should not
be excess globs of grease at any individual point on the ring.
Note: you many want to change gloves after applying the grease to keep from 
getting it on everything else you touch.
After re-greasing, re-insert the O-rings to their original locations and 
re-assemble the vacuum system.
Once everything is set up, activate the pump and monitor the pressure.
If this fixed the problem continue with the pump-down procedure.
If not, continue on the set 3.

### 3. Localize Leak

Up til now we have been treating the vacuum system as a whole.
In my experience, the previous 2 steps have resolved 90% of the issues I've
had with the system.
However, when these steps fail, it is useful to narrow down where specifically
in the vacuum system the problem is occuring: the pump, the hose, or the 
Y-adapter. 
This is easily accomplished by sequentially verifying each component, starting
with the pump.

#### a. Verify Pump

To verify that the turbopump can pull vacuum, remove the cryo-hose from the 
pump and replace the hose with an O-ring and vacuum cap on the pump stem.
Make sure the cap has been sufficiently tightened (use channel locks on the 
clamp).
When you are confident the setup is correct, activate the pump.
If the pump cannot pull vacuum (<1e-7 mbar), then there is likely a problem 
with the pump itself.
You can try re-greasing the O-rings inside the pump (be very careful when
disassembling).
If that doesn't work, notify your advisor.
Assuming that the pump is working as expected, move to the next step.

#### b. Verify hose

Having successfully verified that the pump can pull vacuum, reattach the 
vacuum hose and move the vacuum-cap from the pump stem to the other end of the
vacuum hose.
Re-tighten all clamps and activate the pump.
If vacuum cannot be obtained, replace the vacuum hose and try the procedure
again.
If high-vacuum is obtained, then you have verified that there is no problem 
with either the pump or the hose.
By process of elimination, this leaves the Y-adapter as the likely culprit.
CCI-2 has 2 Y-adapters, so try swapping out for the other one and see if that
fixes the problem.

### 4. It Still Doesn't Work

In my experience, the above procedures have been sufficient to successfully
debug/repair vacuum issues.
If none of the debugging procedures worked or the diagnostics were 
inconclusive, consult with your advisor.
