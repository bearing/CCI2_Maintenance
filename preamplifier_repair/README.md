# Repair and Replacement of Front-End Electronics

CCI-2 is instrumented with ultra-low-noise, high-gain MAFIA charge-sensitive
preampflifiers.
These preampflifiers do not have input protection circuitry, thus the 
first-stage JFET's are easily blown out.
The AC-side is particularly sensitive, as transients on the HV bias line 
can have high-frequency components that pass right through the coupling
capacitor.
Since 2010, CCI-2 has had all the preamps damaged twice 
(necessitating the replacement of the first-stage JFET for all 152 
preamplifiers) while the AC-side preampflifiers have needed replacement at 
least two additional times due to issues with the application of high voltage.
With the acquisition of a better UPS, CCI-2 has not had front-end issues 
since 2014.
Nevertheless, it is a good idea to know how to repair/replace the preamps
should something go wrong.

## Debugging Preamplifier Problems

The simplest way to determine whether the preamplfiers are function or not
without having to disassemble the system is to test whether they respond to 
being powered.

**Make sure the detector is not biased for this procedure!**

With the detector unbiased, simply hook up preamplifier signal channels to the
oscilloscope and toggle the preamplifier power supply (i.e. turn the NIM bin
on/off).
The oscilloscope traces should respond in some way to the application of 
power to the preamplifiers.
The AC-side preamplifiers exhibit a baseline "recovery time" due to the time
constant formed by the coupling capacitor.
If the oscilloscope traces do not respond in any way to power cycling, the
preamplifiers may be damaged.
The only way to tell for sure is to disassemble the preamplifier box and test
the preamplifiers individually.
This procedure is described in 
[this document](./cci2Preamplifiers_TestingAndReplacement.pdf)

## Getting the Preampflifiers Repaired

If you do end up confirming that the preamplifiers are "dead", they will need
to be repaired.
Fortunately, there is a company in the South Bay, Telirite Technical Services,
that can replace the JFETs and clean the boards for a very reasonable price
*much* faster and more reliably than you'd be able to do yourself with the
soldering stations we have available.
I strongly recommend contacting them in the event that the first-stage JFETs 
need to be replaced.
Note that they do not carry the JFETs in stock - you must send the replacement
JFETs along with the boards themselves to be repaired.
Contact your advisor for how to obtain the necessary equipment.

## Procedure for Testing/Replacing Damage Preamplifiers

This procedure is described in detail in 
[this document](./cci2Preamplifiers_TestingAndReplacement.pdf).
