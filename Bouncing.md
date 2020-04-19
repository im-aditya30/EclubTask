# Bouncing & Debouncing

## Bouncing <br>
Bouncing is a phenomenon that occurs whenever a switch is pressed. Whenever a switch is pressed two metal contacts touch each other. Due to physical limitations,these two metal contact have a small amount of space in which they can move freely. When the two contacts touch each other, the contacts don’t stop moving and bounce apart, and touch once again. This may occur multiple times in a single press. The time between each bounce varies a lot but is usually in the range of 10s of microseconds. This is not a issue in everyday circuit as it is too fast for humans to perceive. However, in Electronics,we regularly encounter circuits that work much faster than the bounce time. This result in a single press being register as multiple presses. <br>

## Debouncing<br>
  Since bouncing is a phenomenon that occurs in each and every switch, we cannot remove it. We need to account for it while designing the circuit. Bouncing can be compensated by two methods. <br>

*  **Hardware Debouncing**  
   You can debounce a switch just using a Resistor and Capacitor. The output of the switch should be connected to a [RC low-pass]()*(TODO addLink)* ﬁlter before being connected to the circuit.    
<br>

* **Software Debouncing** 
    Software debouncing works a little differently. Whenever you detect a switch begin pressed, you start a timer for a set duration and ignore the switch’s state for that duration.
<hr>