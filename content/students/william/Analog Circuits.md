---
title: "Analog Circuits"
date: 2021-01-11T19:44:43-06:00
draft: false
---


Series VS Parallel Circuits:

-----------
An Intoduction to Breadboards:

For all the examples below, I am using a breadboard to house my LEDs and complete my circuit, if I was not using
a breadboard, I would be using wires to do the same thing. A breadboard is basically a tool in order to simplify a circuit.

A current will always run heightwise(for this example), or along the numbered columns. This rule works for everything but
the (-) and (+) terminals, in which current runs lengthwise. These two terminals are also specifically for the (+) and (-) charge specifically,
while the numbered rows can be used for either.
----------- 

A series circuit is a circuit that depends on each item in the chain in order for current to flow, making the circuit work.

![image](../images/Series Circuit.png)

Should one item in the circuit be removed or fail, then the whole circuit will be disconnected.
Should this happen, current will not run through it, resulting in nothing happening when connected to a power source.

![image](../images/Series Circuit2.png)

In contrast, a parallel circuit is one that work even if an item is removed. In both situations, the LED lights are the items
being removed. In the series circuit, the circuit is broken with the removal of the LED, causing nothing to happen.

![image](../images/Parallel Circuit.png)

For a parallel circuit, when the LED is removed, the circuit is not broken because it is still connected to the other LEDs,
thus retaining the property of a complete circuit.

![image](../images/Parallel Circuit2.png)
