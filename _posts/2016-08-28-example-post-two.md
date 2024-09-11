---
title: QDC
---

QDC a.k.a a charge to digital converter allows you to measure the charge that passes through it. It comes in all shapes and sizes ranging from an electrical component to the impressive CAEN v792AC (see picture below) that we are using.

![](/assets/images/qdc1.jpeg)

Now let's look at the current at the QDC's input. 

![](/assets/images/qdc2.png)

As you can see, there is a very strong background in addition to the current signal caused by a detector. For the noise to contribute to our reading as little as possible, and also to not lose any of the actual signal, we must pick a very specific integration window. On the picture you can see why the specific $t_{start}$ and $t_{end}$ were chosen.
The green signal here is a trigger signal, it functions as a gate. When it goes `LOW`, the gate closes and current flows onto one plate of the capacitor. An uncharged capacitor initially acts as a wire, so a fast-enough current signal coming through the gate will simply pass through the capacitor, during which charge accumulates on the capacitor. Then, when the gate closes and the capacitor has just reached its maximum voltage, the ADC comes in to measure that voltage. Here an ADC is just used as a voltmeter. 

![](/assets/images/qdc3.png)
What opens and closes the gate? It is a so-called gate generator that gets the signal somewhat earlier than the other components. This is because the signal is delayed before it reaches the gate. The gate generator then recognizes the rise in current and it opens the gate just in time for the signal to arrive at the gate.  On the drawing, there is not only $I(t)$ - our signal coming into the gate. There is also the pedestal current $I_{PED}$ – a constant current which is also fed into the QDC. 
Its purpose is to reduce the relative error on the ADC reading (I'm not sure why this is important, since after subtracting the pedestal current in data analysis, the relative error will still be the same) and to bring the capacitor into a mode where it is working linearly, i.e where the effective capacitance is the nominal one. 

![](/assets/images/qdc4.png)

