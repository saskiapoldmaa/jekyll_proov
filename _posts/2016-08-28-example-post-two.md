---
title: QDC
---

QDC is a charge to digital converter. This allows you to measure charge that flows through the QDC. 

![](/assets/images/qdc1.jpeg)

The graph above depicts the current through the QDC. As you can see, the signal is not at completely 0 when there is no signal, this is due to the noise. For the noise to not contribute, we must pick a very specific integration window, so that only the charge that flew between t\_start and t\_end will be measured.

![](/assets/images/qdc2.png)

The green signal here is a trigger signal, it functions as a gate. When it goes LOW, the gate closes and current flows onto one plate of the capacitor. An uncharged capacitor initially acts as a wire, so a fast-enough current signal coming through the gate will simply pass through the capacitor, during which charge accumulates on the capacitor. Then, when the gate closes and the capacitor has just reached its maximum voltage, the ADC comes in to measure that voltage. Here an ADC is just used as a voltmeter. 

![](/assets/images/qdc3.png)
What opens and closes the gate? It is a so-called gate generator that gets the signal somewhat earlier than the other components. This is because the signal is delayed before it reaches the gate. The gate generator then recognizes the rise in current and it opens the gate just in time for the signal to arrive at the gate.  On the drawing, there is not only I(t) - our signal coming into the gate. There is also I\_PED - a pedestal current. Its purpose is to get a smaller relative error on the ADC reading and to bring the capacitor into a mode where it is working linearly, i.e where the effective capacitance is the nominal one. 

![](/assets/images/qdc4.png)

