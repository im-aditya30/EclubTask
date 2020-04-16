# Basic Electronics
//inductor,capacitor,jumper,normalwire,potentiometer,resistor,ics,colorcoding,ceramic capaitors coding also,
## BreadBoard
 **What is a BreadBoard ?**<br><br>
 A breadboard is a rectangular plastic board with a bunch of tiny holes in it. These holes let you easily insert electronic components to prototype (meaning to build and test an early version of) an electronic circuit, like this one with a battery, switch, resistor, and an LED (light-emitting diode). The connections are not permanent, so it is easy to remove a component if you make a mistake, or just start over and do a new project.<br><br>
 **How are the Holes inside breadboard connected ?**<br><br>
 The leads of wires or any other component can fit into the breadboard beca3use the inside of a breadboard is made up of sets of five metal clips. This means that each set of five holes forming a half-row (columns A–E or columns F–J) is electrically connected.  
 For example, that means hole A1 is electrically connected to holes B1, C1, D1, and E1. It is not connected to hole A2, because that hole is in a different row, with a separate set of metal clips. It is also not connected to holes F1, G1, H1, I1, or J1, because they are on the other "half" of the breadboard—the clips are not connected across the gap in the middle (to learn about the gap in the middle of the breadboard, see the Advanced section). Unlike all the main breadboard rows, which are connected in sets of five holes, the buses typically run the entire length of the breadboard (but there are some exceptions).   <br>
<p align ="center">
 <img align="center" src="/images/breadboardconnections.png" alt="Breadboard"><br><br>
  Above image shows which holes are electrically connected in a typical half-sized breadboard, highlighted in yellow lines.
</p> <br>
  

## Bouncing

 1. **Bouncing**<br><br>
Bouncing is a phenomenon that occurs whenever a switch is pressed. Whenever a switch is pressed two metal contacts touch each other. Due to physical limitations,these two metal contact have a small amount of space in which they can move freely. When the two contacts touch each other, the contacts don’t stop moving and bounce apart, and touch once again. This may occur multiple times in a single press. The time between each bounce varies a lot but is usually in the range of 10s of microseconds. This is not a issue in everyday circuit as it is too fast for humans to perceive. However, in Electronics,we regularly encounter circuits that work much faster than the bounce time. This result in a single press being register as multiple presses.

 1. **Debouncing**<br><br>
  Since bouncing is a phenomenon that occurs in each and every switch, we cannot remove it. We need to account for it while designing the circuit. Bouncing can be compensated by two methods.
     *  Hardware Debouncing<br>
   You can debounce a switch just using a Resistor and Capacitor. The output of the switch should be connected to a RC low-pass ﬁler   before being connected to the circuit.
     * SoftwareDebouncing <br>
    Software debouncing works a little differently. Whenever you detect a switch begin pressed, you start a timer for a set duration and ignore the switch’s state for thatduration.

## Pull Up and Pull Down Resistors  <br>
 When working with digital circuits, one needs to make sure that every input is clearly deﬁned in the form of a particular value: either HIGH or LOW.If the inputs of the digital circuit are not with in the range of values by which they can be clearly separated as HIGH or LOW triggers,then it may lead to the sensing of a false trigger or self bias that will lead to the  circuit not working properly.<br>
<p align = "center>
      <img src = "/images/PullUPAndDown.gif" alt="Figure 1:Example"><br>Figure1:Example   
</p>
  For example, consider the digital circuit above(Fig.1). The two switches, “a” and “b”, represent the inputs to a generic logic gate. When switch “a” is closed (ON), input “A” is connected to ground, (0v) or logic level “0” (LOW) and likewise, when switch “b” is closed (ON), input “B” is also connected to ground, logic level “0” (LOW) and this is the correct condition we require.However, when switch “a” is opened (OFF), what will be the value of the voltage applied to input “A”, HIGH or LOW?<br><br>
  We assume it will be +5V (HIGH) as switch “a” is open-circuited and therefore input “A” is not shorted to ground, but this may not be the case. As the input is now effectively unconnected from either a defined HIGH or LOW condition, it has the potential to “float” about between 0V and +5V (Vcc) allowing the input to self–bias at any voltage level whether that represents a HIGH or a LOW condition. This may lead to an open(HIGH) switch to be assessed as a closed(LOW) switch that may lead to a change in the output that is obtained at the logic output(Q).<br><br>
    Then to prevent accidental switching of digital circuits, any unconnected inputs called ﬂoating inputs should be tied to a logic 1 or logic 0 as appropriate for the circuit. We can easily do this by using what are commonly called Pull-up Resistors and Pull-down Resistors to give the input pin a deﬁned default state, even if the switch is open, closed or there is nothing is connected to it.<br> <br>
   1. **Pull Up Resistor Application** <br><br>
  By using these two pull-up resistors, one for each input, when switch A or B is open (OFF), the input is effectively connected to the +5V supply rail via the pull-up resistor. The result is that as there is very little input current into the input of the logic gate, very little voltage is dropped across the pull-up resistor so nearly all the +5V supply voltage is applied to the input pin creating a HIGH, logic 1 condition.
  When switches A, or B are closed, (OFF) the input is shorted to ground (LOW) creating a logic 0 condition as before at the input.We are not shorting out the supply rail as the pull-up resistor only passes a small current (as determined by Ohms law) through the closed switch to ground. If we do not use a resistor then a high value of current will pass through the circuit and that could damage the electronic devices involved in the circuit.
  By using a pull-up resistor in this way, the input always has a default logic state, either 1 or 0, high or low, depending on the position of the switch, thus achieving the proper output function of the gate at Q and therefore preventing the input from ﬂoating about orself-biasing giving us exactly the switching condition we require.<br><br>
   2. **Pull Down Resistor**<br>
  A Pull-down resistor works in the same way as the previous pull-up resistor, except this time the logic gates input is tied to ground, logic level 0(LOW) or it may go HIGH by the operation of a mechanical switch. This pull-down resistor conﬁguration is particularly useful for digital circuits like latches, counters and ﬂip-ﬂops that require a positive one shot trigger when a switch is momentarily closed to cause a state change.<br>

 For More About Pull Up & Down Resistor [click Here](https://www.electronics-tutorials.ws/logic/pull-up-resistor.html) <br><br>
## Logic Gates
   **What are Logic Gates?**<br><br>
   Logic gates are the basic building blocks of any digital circuit. They are electronic circuits which have one or more inputs and only one output which relates to the input signals based on a certain logic.<br>
  These are the basic logic gates:<br>
   * AND Gate<br>
 [![AND Gate  Symbol](/images/andgate.png "AND Gate")](https://www.electronicshub.org/digital-logic-and-gate/) <br>
   * OR Gate<br>
 [![OR Gate Symbol](/images/orgate.png "OR Gate")](https://www.electronicshub.org/digital-logic-or-gate/) <br>
   * NOT Gate<br>
 [![NOT Gate  Symbol](/images/notgate.png "NOT Gate")](https://www.electronicshub.org/digital-logic-not-gate/) <br>
   * NOR Gate<br>
 [![NOR Gate Symbol](/images/norgate.png "NOR Gate")](https://www.electronicshub.org/universal-gates-nor-gate/) <br>
   * NAND Gate<br>
 [![NAND Gate Symbol](/images/nandgate.png "NAND Gate")](https://www.electronicshub.org/universal-gates-nand-gate/) <br>
   * XOR Gate<br>
 [![XOR Gate Symbol](/images/exorgate.png "XOR Gate")](https://www.electronicshub.org/exclusive-or-gatexor-gate/) <br>
   * XNOR Gate<br>
  [![XNOR Gate Symbol](/images/xnorgate.png "XNOR Gate")](https://www.electronicshub.org/exclusive-nor-gate/) <br>
 ##### The NAND (NOT-AND) and NOR (NOT-OR) gates are considered universal gates and can be used to make any other logic gate.<br> For example : NAND gate can be use to make following gates:<br>
 ![NAND Gate Applications](/images/nandgateUses.webp)

  
source:
  * [Eclub Manual](/handbook/handbook.pdf)
  * https://www.electronicshub.org/
