## VLSI Skill Assessment 

## Common-Drain-Amplifier Design and Implementation using Cadence EDA Tools

## Abstract
To design and implement a Differentiator Amplifier circuit using Cadence EDA tools, simulate its functionality,Key performance metrics such as gain, common-mode rejection ratio (CMRR), and bandwidth are analyzed through schematic and post-layout simulations. The results demonstrate the effectiveness of Cadence Virtuoso in optimizing analog circuit design for high-performance applications.

## Circuit Design
![1481278107](https://github.com/user-attachments/assets/83781705-3e2c-41b8-816a-abb07964679b)


## Circuit Description
A differentiator amplifier is a type of analog circuit that produces an output voltage that is proportional to the rate of change (derivative) of the input voltage. It is typically implemented using an operational amplifier (op-amp) in an inverting configuration with a specific combination of resistors and capacitors.

## Getting Started Setting Up Cadence Virtuoso Open Terminal:

Right-click and open the terminal window. Enter the following commands: sh Copy code csh source /cadence/install/cshrc virtuoso

## Creating New Library & Schematic:

Library: File -> New -> Library, name it (e.g., VLSILAB_EXP_2), and attach it to the technology library gpdk045. Schematic Cell View: Go to File -> New -> Cell View, set up the library, cell, and view as follows: Library: Select your created library. Cell Name: E.g., diff amplifier_sche. View: Schematic. Adding Components and Connections:

Use the instance tool to add components such as nmos1v and pmos1v. Add input and output pins, and make all connections using the wire tool.
![1](https://github.com/user-attachments/assets/1854dce9-319c-4992-8aa1-7a08f3d83704)


## Symbol Creation:

Go to Create -> Cell View -> From Cell View to generate the symbol automatically. Customize the symbol if needed. Simulation with Spectre Set Up Simulation: 

![2](https://github.com/user-attachments/assets/d7565733-4832-49b3-94b7-9e2e90fdfb5c)


Use symbol to make circuit 

![3](https://github.com/user-attachments/assets/ce643389-2353-4c75-8c4c-f64077290636)


Launch ADE L (Analog Design Environment). Set the simulation to Spectre and configure settings in Setup -> Simulation Directory/Host. Specify Analysis Type:

![4](https://github.com/user-attachments/assets/6e56c26d-56f2-48d9-8d1d-e179f0fd06aa)


Use Analysis -> Choose to configure settings for DC sweep or AC sweep or transient
Simulate the Common Drain Amplifier circuit.

## Results of simulation
After simulation, verify the expected characteristics of the Differential amplifier. The simulation should demonstrate the following:
Input Signal: The input is typically a sinusoidal or step signal.
Output Signal: The output is the derivative of the input signal, ideally displaying a sharp change corresponding to the rate of change of the input.
Expected Behavior:
For a sinusoidal input, the output should be a sinusoidal signal that is 90° out of phase with the input and scaled by the factor RC.
For a step input, the output should exhibit a pulse corresponding to the rate of change of the step.
![5](https://github.com/user-attachments/assets/fad57dbb-bfbc-49f3-953b-8cdbc7fcea54)

## Conclusion
The design and simulation of the Differential Amplifier using Cadence EDA tools were successful
