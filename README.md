# Reconfigurable Flight Controller SoC for UAVs
### Abstract
UAVs such as drones are becoming more and more ubiquitous and consequently are being utilized in quite a lot of novel applications for which the traditional microcontroller based flight controllers may not be adequate. This requirement has been recognized and many FPGA based flight controllers such as [PynqCopter](https://github.com/UCSD-E4E/pynq-copter), [Aerotenna](https://aerotenna.com/ocpoc-cyclone/) etc. have surfaced which capitalize on the parallelism capabilities of FPGAs to deliver performance that is, at least in theory, superior to the microcontroller based counterparts.

For any FPGA based system, the next leap in performance is achievable through ASIC fabrication. However, flight controllers need to interface with different types and different number of sensors based on the application at hand. Thus, a frozen chip would be quite unappealing and impractical since it would limit the user to a single, or at best a set of, fixed sensor configurations.

We therefore propose a reconfigurable system-on-chip (SoC), containing the features common to most flight controllers (such as PID controllers, I2C and SPI peripherals etc.) as hard blocks, and a reconfigurable fabric based on the [OpenFPGA](https://github.com/lnis-uofu/OpenFPGA) project allowing the user to develop their own sensor interface, fusion and processing IPs, depending on their specific requirements.
### Block Diagram
A basic block diagram of the proposed chip is shown below.
![alt text]()
