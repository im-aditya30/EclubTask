# Basic Electronics

## Bouncing

1. **Bouncing**<br><br>
Bouncing is a phenomenon that occurs whenever a switch is pressed. Whenever a switchispressedtwometalcontactstoucheachother. Duetophysicallimitations,these two metal contact have a small amount of space in which they can move freely. When the two contacts touch each other, the contacts don’t stop moving and bounce apart, and touch once again. This may occur multiple times in a single press. The time between each bounce varies a lot but is usually in the range of 10s of microseconds. This is not a issue in everyday circuit as it is too fast for humans to perceive. However, in Electronics,we regularly encounter circuits that work much faster than the bounce time. This result in a single press being register as multiple presses.

1. **Debouncing**<br><br>
  Since bouncing is a phenomenon that occurs in each and every switch, we cannot remove it. We need to account for it while designing the circuit. Bouncing can be compensated by two methods.
    *  Hardware Debouncing<br>
   You can debounce a switch just using a Resistor and Capacitor. The output of the switch should be connected to a RC low-pass ﬁler   before being connected to the circuit.
    * SoftwareDebouncing <br>
    Software debouncing works a little differently. Whenever you detect a switch begin pressed, you start a timer for a set duration and ignore the switch’s state for thatduration.

1. **Pull Up and Pull Down Resistors**  <br><br>
When working with digital circuits, one needs to make sure that every input is clearly deﬁned in the form of a particular value: either HIGH or LOW.If the inputs of the digital circuit are not with in the range of values by which they can be clearly separated as HIGH or LOW triggers,then it may lead to the sensing of a false trigger or self bias that will lead to the  circuit not working properly.<br>
  ![Figure 1: Example](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.electronics-tutorials.ws%2Flogic%2Fpull-up-resistor.html&psig=AOvVaw35ffzYVlqwqGes57PZxYto&ust=1586983067349000&source=images&cd=vfe&ved=0CAIQjRxqFwoTCNDT9OXi6OgCFQAAAAAdAAAAABAD) <br>
  For example, consider the digital circuit above(Fig.1). The two switches, “a” and “b”, represent the inputs to a generic logic gate. When switch “a” is closed (ON), input “A” is connected to ground, (0v) or logic level “0” (LOW) and likewise, when switch “b” is closed (ON), input “B” is also connected to ground, logic level “0” (LOW) and this is the correct condition we require.However, when switch “a” is opened (OFF), what will be the value of the voltage applied to input “A”, HIGH or LOW?<br><br>
  We assume it will be +5V (HIGH) as switch “a” is open-circuited and therefore input “A” is not shorted to ground, but this may not be the case. As the input is now effectively unconnected from either a defined HIGH or LOW condition, it has the potential to “float” about between 0V and +5V (Vcc) allowing the input to self–bias at any voltage level whether that represents a HIGH or a LOW condition. This may lead to an open(HIGH) switch to be assessed as a closed(LOW) switch that may lead to a change in the output that is obtained at the logic output(Q).<br><br>
    Then to prevent accidental switching of digital circuits, any unconnected inputs called ﬂoating inputs should be tied to a logic 1 or logic 0 as appropriate for the circuit. We can easily do this by using what are commonly called Pull-up Resistors and Pull-down Resistors to give the input pin a deﬁned default state, even if the switch is open, closed or there is nothing is connected to it.<br> <br>
    * Pull Up Resistor Application
    By using these two pull-up resistors, one for each input, when switch A or B is open (OFF), the input is effectively connected to the +5V supply rail via the pull-up resistor. The result is that as there is very little input current into the input of the logic gate, very little voltage is dropped across the pull-up resistor so nearly all the +5V supply voltage is applied to the input pin creating a HIGH, logic 1 condition.


