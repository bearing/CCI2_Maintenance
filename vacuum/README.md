# Vacuum Systems for CCI-2

Common with all HPGe cryostats, the CCI-2 cryostat must be kept at vacuum.
This is essential for being able to reach and maintain cryogenic temperatures,
and is also important for the detector itself.
Even when the detector is not in use and not cooled, the vacuum in the cryostat
should be maintained.

## General Overview

The CCI-2 cryostat is kept at vacuum, typically less than 1e-6 mbar.
The vacuum is achieved by means of a turbopump and is passively maintained
while the detector is operation (i.e. there is no pump running while the
detector is in use.
In principle, there is an ion pump mounted in the cryostat which can help
maintain the vacuum during periods between active "pump-downs" with the 
turbopump, but the ion pump has never been used as I was never able to find
all of its associated equipment (power supply, etc.)

There is pressure gauge that records the pressure inside the cryostat directly.
When the detector is cooled, the temperature serves as a proxy for the 
indirect measurement of pressure in the cryostat (ideal gas law).
As such, rapid changes (i.e. increases) in temperature (on the order of 1K per
10s or faster) indicate a loss of vacuum.

The vacuum in the CCI-2 cryostat has been continually maintained since 2010
without any major breaches.
Note that this means the O-rings in the cryostat are nearly a decade old and
have not received any attention in nearly a decade.
According to manufacturer datasheets, the O-rings used in the CCI-2 cryostat
have a shelf-life of about 10 years; it would not be surprising for there to
be an O-ring failure in the near future.
In the event of an o-ring failure (or complete loss of vacuum by other means),
it is recommended that the cryostat be opened and all internal vacuum 
components be replaced.

## When to Pump

As there is no active maintenance of the cryostat vacuum when CCI-2 is in 
operation, it tends to slowly degrade over time.
This most clearly manifests in a slow rise in the minimum achievable cryostat
temperature over time. 
Immediately following a pump-down, a minimum temperature of around 91K is 
typically achieved.
The minimum achievable temperature tends to rise at a rate on the order of
1K per month.
It is recommended that CCI-2 only be operated at temperatures below 96K (see
overview), thus CCI-2 should be pumped-down once every 3-4 months during 
normal use.

## Working with Vacuum Components

There are some important considerations that should be kept in mind when 
working with vacuum components.
The most important is: **wear gloves!**
Latex/nitrile gloves should be worn whenever you are handling components that 
are to be kept under vacuum.
The natural oils from your skin will contaminate the components making vacuum
more difficult or in some cases impossible to obtain.
In the event that you do accidentally touch a piece of equipment with bare
skin, or it needs to be cleaned for any other reason, there is an ultrasonic
cleaning station in 1110B that can be used to clean small metallic components.
Rubber/plastic components should be replaced rather than cleaned.

Like everything else with CCI-2, it pays to work methodically and carefully
with the vacuum components.
Never force the coupling of threaded components if you feel resistance - 
forcing misaligned threads can damage the equipment.
Always double check that there are O-rings at the connections between all 
components you are hooking up (hoses, flanges, etc) and visually inspect them
to make sure they are not "pinched" or damaged in any visible way.
O-rings tend to dry out and need to be re-greased from time to time.
If you are having trouble attaining/maintaining high vacuum, this is the first
place to look.

## Procedure for CCI-2 Pump Down

As noted above, CCI-2 needs to be actively "pumped down" using the turbopump
about once every 3-4 months.
The pump down procedure can be found [here](./pump_down_procedure.md).
