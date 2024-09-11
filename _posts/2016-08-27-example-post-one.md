---
title: Cherenkov detector
categories:
- General
- External sources
feature_image: "https://picsum.photos/2560/600?image=872"
---
![Basic Cherenkov](/assets/images/xcet.gif)

Cherenkov detectors, also known by the abbreviation XCET, are gas-filled detectors capable of determining if a charged particle passing through them is above a certain cutoff momentum. If the particle is faster than the phase velocity of light in that gas, the gas will emit light (the principle that nothing can be faster than light applies only to the group velocity of light, not the phase velocity).

The threshold momentum is regulated by the pressure in the detector. The higher the pressure, the higher the refractive index and the slower the light travels in that medium. Hence, to increase the threshold momentum for particles, you need to decrease the pressure.

When you combine two Cherenkov detectors at two different pressures, i.e., you have two different momentum cutoffs for particles to emit light, then you can identify all of the particles in the momentum range specified by the cutoff momenta of each of the detectors. A particle will fall into that momentum range if it emits light in one of the Cherenkov detectors but not in the other.

To map out the momentum of all the particles in the beam, i.e., to measure a spectrum, you need to perform a so-called pressure scan. For this, only one Cherenkov detector is necessary, but you need to vary the pressure in it from the maximum to the minimum. This can be done by initially pumping the detector full of gas and taking measurements while it gradually depressurizes.

During pressure scans, you usually measure the # of particles in a spill that made the medium emit light. You can compare this to the total number of particles in that spill, which is given by the trigger rate.
![Pressure scan](/assets/images/che.png)

The x-axis represents the pressure in the Cherenkov detector in bars. On the y-axis is the Cherenkov efficiency.
Cherenkov efficiency is not really an efficiency; it is actually the ratio of particles that emit light to the total number of particles (trigger rate).

As you can see, at low pressure, the threshold momentum is very high, so there are few particles that actually get detected, but as the pressure increases, the momentum becomes less and less discriminating, so more particles are detected.

Pressure scans are more useful after you've translated the x-axis from pressure to threshold momentum.Because particle energies usually follow a normal distribution, the 50% efficiency usually responds to the peak of the spectrum.
![Pressure scan after calculations](/assets/images/pre.png)
