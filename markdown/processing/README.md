Radiometer Info

What it does: Uses directional radio waves from an antenna to find the potential of the surface it's pointed at, which can then be used to determine the substance's moisture level. (e.g. determining moisure of soil over an area; cloud detection)

Required components:
-Antenna and receiver that measures power
-Bandpass filter
-Transformer to convert impedance (Balin type? I cannot read exactly what my notes say here)
-LNA and ADC

Antenna:
Needs to be more focused and directional; high frequency. A horn would be the most accurate option but too large and expensive. We should build a reflector antenna (dish with a dipole feed) instead. This would be small enough to fit the size of the PocketQube, though we would have to rework one of the exterior PCBs to allow it to sit sort of inside the design. Some useful values are a Coax of 50Ohms and Dipoles of 300Ohms. We would need to calculate the concavity of the dish shape and find the focal/center point of it to place the dipole feed at.

Frequency:
The frequency we attenuate to must be high. 376Hz is about the frequency of clouds. 196Hz should also be a good one to measure at. We also have to make sure that the frequency we use is an allowed one to measure signals across that no one can broadcast on.

Equations:
Pm = P + Pn     (with Pn being noise power)
T = E*Tp        (with E being emissivity)
P = k*I*B
Beam length is lambda/d (in radians; with d being the dimensions of the antenna)
We want to have an f/d of about 1

Other info:
We can estimate the noise power by pointing the antenna at a calibration source (e.g. the clear sky).
I drew some diagrams and pictures in my notes while talking to Dr. Long that may be helpful as well, but I cannot put them in the README.