Download Link: https://assignmentchef.com/product/solved-ece2220-lab2-quartus-ii-and-the-de10-designing-a-simple-logic-circuit
<br>
The purpose of this lab is allow you to become more familiar with Quartus® II, the simulation software, programming of the DE10 Standard board and the design of a simple combinational logic circuit.

<h1>2) Instructions</h1>

<ol>

 <li>Derive the truth table of the problem corresponding to logic problem described below.</li>

 <li>Find the simplified circuit corresponding to the truth tale and draw it on the answer sheet.</li>

 <li>Using Quartus® II, write the Verilog code for your circuit.</li>

 <li>Simulate the code and show the result to the TA.</li>

 <li>Program the hardware and show the result to the TA.</li>

</ol>

<h1>3)The Logic Problem</h1>

A washing machine motor is turned on by a control circuit. The circuit checks following conditions,

<ul>

 <li>Power switch is ON ( Logic 1: ON , Logic 0: OFF)</li>

 <li>Door is locked (Logic 1: Locked, Logic 0: Unlocked)</li>

 <li>Water level is high enough (Logic 1: High, Logic 0: Low)</li>

 <li>Over flow limit ( Logic 1: Above Overflow, Logic 0: Below Overflow)</li>

</ul>

The motor is turned on only if all the above conditions are met. Build a logic circuit for this washing machine control circuit.

<ol>

 <li>Produce a truth table for this circuit</li>

 <li>Sketch the simplified circuit</li>

 <li>Write the Verilog code</li>

 <li>Run a “functional” simulation of the hardware and show the timing diagram. <strong> </strong></li>

 <li>Program DE10 – Standard board and show the working circuit to the TA. The circuit should use the right most 4 LEDs – LEDR[0], LEDR[1], LEDR[2], LEDR[3]) to show the state of each input switch. The left most LED – LEDR[9] should be used for the output. Make sure your code is annotated.</li>

</ol>




<ol>

 <li>Using the right most push button KEY[0], create an automatic/emergency shutoff for the circuit above. When the button is depressed and held for a second or two, the output (i.e. motor power) should be set to zero. The corresponding LEDs should reflect this change. Use LED[5] to show the last state of the pushbutton (i.e. if the button is pushed LED[5] should be on). Once the button is released, the power should remain off until the button is pressed and held a second time. The 2nd push will allow the circuit to restart and operate again based on the input switches Program the DE10 board and show the working circuit to the TA. The bush button are defined by “negative” logic: when pushed the value of KEY[0] goes from high to low and vice versa. Therefore the sensitivity list of the always block used to detect the change in the level.</li>

</ol>


