# 10-bit-current-steering-DAC


The current-steering DAC replaces the resistor element in the resistor DAC architectures with a MOSFET current element and uses some form of summation of the current elements to produce the result. Sometimes the result needs to be a current such as in integrated bias circuits. A current mirror is a circuit designed to copy a current through one active device by controlling the current in another active device of a circuit, keeping the output current constant regardless of loading. The current being "copied" can be, and sometimes is, a varying signal current. Current mirror is used to implement individual current sources of 0.1uA, 0.2uA, 0.4uA, 0.8uA,1.6uA, 3.2uA, 6.4uA, 12.8uA, 25.6uA, 51.2uA. These current sources are driven by a current amplifying circuit through a NMOS (N-channel Metal Oxide Semiconductor) switch, which acts as the digital input. The current amplifying circuit used here is also a current mirror circuit itself.


From the simulation results, we can conclude that the output resistance (ro) of the PMOS in the load side of current amplifier circuit increases as the current flowing through that decreases. Due to increase in the ro, the effective load resistance increases, which alters the output voltage (Vds). When there is lower current flowing through the load, ro is large and produces larger variations in the output voltage (Vds). This is why we could see larger variations of output voltage (Vds) from the ideal value for lower currents (LSB’s are made high) than for larger currents (MSB’s are made high).


The problem stated is corrected using cascoded current mirror amplifiers at the output.
