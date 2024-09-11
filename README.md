# Water-treatment-with-hydrostatic-level-sensor

This repository contains the project of a water deposit with height of 10m. It also has 3 pumps which distribute water to a village. Water will be distributed when a certain level in the water-depo is reached. An analog level sensor (Hydro static) is used in order to measure the water level in the depo.

The system operate as follows:

- When the water level is below 2m , no pump engage.
- When the water level is between [2-5]m the first pump engage.
- When the water level is between [6-8]m the first and the second pump engage.
- When the water level is between [9-10] the first, second and third pump engage.
- The system contains one start, and one stop push-buttons.
- Each pump overload signal is connected to the PLC.
- When an overload occurs, only the corresponding pump stop.
- A log for each pump record the number of faults that has occurred.
- The log reset every 3 days (For simulation purposes every 1 min).
- The analog sensor signal will come in form of [400-20000] so it needs to be scaled to [0-10]m.
