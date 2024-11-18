## VLSI Skill Assessment 

## Common-Drain-Amplifier Design and Implementation using Cadence EDA Tools

## Abstract
To design and implement a Differentiator Amplifier circuit using Cadence EDA tools, simulate its functionality,Key performance metrics such as gain, common-mode rejection ratio (CMRR), and bandwidth are analyzed through schematic and post-layout simulations. The results demonstrate the effectiveness of Cadence Virtuoso in optimizing analog circuit design for high-performance applications.

## Circuit Design


## Circuit Description
A differentiator amplifier is a type of analog circuit that produces an output voltage that is proportional to the rate of change (derivative) of the input voltage. It is typically implemented using an operational amplifier (op-amp) in an inverting configuration with a specific combination of resistors and capacitors.

## Getting Started Setting Up Cadence Virtuoso Open Terminal:

Right-click and open the terminal window. Enter the following commands: sh Copy code csh source /cadence/install/cshrc virtuoso

## Creating New Library & Schematic:

Library: File -> New -> Library, name it (e.g., VLSILAB_EXP_2), and attach it to the technology library gpdk045. Schematic Cell View: Go to File -> New -> Cell View, set up the library, cell, and view as follows: Library: Select your created library. Cell Name: E.g., diff amplifier_sche. View: Schematic. Adding Components and Connections:

Use the instance tool to add components such as nmos1v and pmos1v. Add input and output pins, and make all connections using the wire tool.
![Screenshot 2024-11-11 190958](https://github.com/user-attachments/assets/52989d6c-d832-472a-9057-e7921ebf8034)

## Symbol Creation:

Go to Create -> Cell View -> From Cell View to generate the symbol automatically. Customize the symbol if needed. Simulation with Spectre Set Up Simulation: 

![Screenshot 2024-11-11 190950](https://github.com/user-attachments/assets/ca19063c-efa5-4e96-95a4-8fc0421b8ecd)

Use symbol to make circuit 

![Screenshot 2024-11-11 190937](https://github.com/user-attachments/assets/3a93ecbf-4131-4a77-9cee-89e03e7b94de)

Launch ADE L (Analog Design Environment). Set the simulation to Spectre and configure settings in Setup -> Simulation Directory/Host. Specify Analysis Type:

![Screenshot 2024-11-11 190923](https://github.com/user-attachments/assets/4efafcda-a348-4951-9c85-cf6ecfd2043b)

Use Analysis -> Choose to configure settings for DC sweep or AC sweep or transient
Simulate the Common Drain Amplifier circuit.

## Results of simulation
After simulation, verify the expected characteristics of the common drain amplifier. The simulation should demonstrate the following:
High Input Impedance: Verify minimal loading on the signal source.
Low Output Impedance: Confirm efficient driving capability for subsequent stages.
Unity Voltage Gain (or Slightly Less): Ensure the output voltage closely follows the input signal.

![Screenshot 2024-11-11 190902](https://github.com/user-attachments/assets/871a38fd-e495-400b-bd49-14a0a11ac117)


## Conclusion
The design and simulation of the Common Drain Amplifier using Cadence EDA tools were successful, confirming its impedance buffering properties and suitability for applications requiring high input impedance and low output impedance.
