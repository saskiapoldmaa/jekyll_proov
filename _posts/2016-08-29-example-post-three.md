---
title: The inseparable DWC and TDC
---
For more technical questions refer [here](https://cds.cern.ch/record/702443/files/sl-note-98-023.pdf)

DWCs are gas-filled rectangular chambers that help you track a particle - or at least get their position at the moment they pass the detector. They work like this: a particle passes the gas-filled (argon & $CO_2$) chamber. If the particle is charged, it will ionize the gas inside. In the chamber there are multiple layers of parallel wires, each layer acting as an electrode and neighbouring layers being oppositely charged. 
The positive ions and electrons, which were created in the ionization, will start to move towards their respective electrodes (electrons towards anode and ions towards cathodes). They're not only moving towards the electrodes, they are also accelerating due to the Coulomb force – especially electrons, which reach such a high velocity, that they start to ionize the surrounding gas even further, creating an avalanche (more specifically a Townsend avalanche). Eventually all of the kicked out electrons reach the anode and cause a great current in it. This current in the anode (more specifically its magnetic field) will go on to create an image current* in the cathode. This step is important, because it's not the anode current that we are measuring, it's instead the image current in the cathode. Also, the current will be produced in 2-3 cathode wire, closest to the anode wire where avalanche took place.
Neighbouring cathode wires are connected to each other with little delay lines. The two edgemost wires are connected to a sensor. The current that passes the sensor has a characteristic mountain shape in time.
<details>
<summary>*</summary>
<br>
image/mirror current here is just the current which the magnetic field of the neighbouring electrode produced in our cathode. The words "image" or "mirror" are used because it turns out that as far as the magnetic field is concerned, the current inside our electrode can be modelled as a reflection of the anode, where the mirror is the surface of our cathode.
</details>
Each step is the contribution from a single wire. They add up at various times thanks to the delay lines, but this is not really the important part. The delay lines are actually there so that the little current mountain would reach the two detectors at opposite sides of the cathode at different times. The moment when the signal is detected is not at the peak of the mountain, it is at the rising edge.
The time interval between signal arrivals is all that is needed to find where the particle passed through.

