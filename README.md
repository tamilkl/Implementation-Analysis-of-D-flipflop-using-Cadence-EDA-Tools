### Ex No: 03    Implementation & Analysis of D-flipflop using Cadence EDA Tools   

### Aim:
To design and implement a D-flip-flop using Cadence EDA tools, simulate its behavior, and analyze key performance parameters such as timing, power consumption, and resource utilization for a comprehensive understanding of sequential logic circuits.

### Tools Required:<br>
•	Personal Computer<br>
•	Cadence Virtuoso Software<br>

### S C H E M A T I C S I M U L A T I O N - PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION -Commands to get into Cadence

1.	Right Click and open the terminal window.<br>
2.	Type the following commands as follows and press enter.<br>
•	csh<br>
•	source /cadence/install/cshrc<br>
•	virtuoso <br>
### Procedure for Schematic simulation using Cadence

1.	Now two windows must open i) virtuoso/command interpreter window<br> ii)”Whats New…”<br>
2.	Close the 2nd window<br>
3.	Use 1st window i.e virtuoso window (CIW) for further processing.<br>
i.	Create a New Library<br>
ii.	Create Schematic Cell view.<br>
iii.	Create the Symbol for schematic Cell view.<br>
iv.	Create the test Cell view.<br>
v.	Analog simulation by spectre<br>


### i)	Procedure for Creating New Library.
•	File –New – Library<br>
•	Name: Give name for ur library Ex: VLSILAB_EXP_1<br>
•	Enable Attach to an existing technology library, Click OK<br>
•	Attach the library to the technology library gpdk045.Click OK<br>
### ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso (CIW)<br>
•	File-New-Cell view<br>
•	Setup the new file form<br>
	Library: Select the one you created.<br>
	Cell: Give the experiment name Ex: Inverter ViewSchematic<br>
	Type: Schematic press OK<br>
•	Add the required components from the libraries and make the connections.<br>
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances<br>
	Click on browse. This opens the library browser<br>
	Now select the appropriate library for components like
	Gpdk45 ------------------------nmos1v, pmos1v
	Create Input and Output pins<br>
	Make the connections by using fixed narrow wire key<br>
	Click Check and Save button
![image](https://github.com/user-attachments/assets/7505eb4b-483f-444b-bc88-0233dbd62a6f)




 
### iii)	Creating the Symbol for schematic Cell view

•	In the schematic window, execute<br>
	Create – Cell view – From Cell view<br>
	The cell view from cell view window appears<br>
	Check Lib Name, Cell Name, From View name must be schematic Press ok<br>
•	Now Symbol generation form appears. Click Ok If No changes required<br>
•	A new window with with default symbol is created.<br>
•	Edit the symbol if you want to give actual symbol shape else continue.<br>
•	Execute Create-Cell view-from cell view<br>
•	Library Name and Cell Name must be same which you have used for schematic. Press OK<br>
•	Check for the position of pin side.Prss <br>
•	Edit for the shape by Create-Shape-Choose required options to edit.<br>

![image](https://github.com/user-attachments/assets/e5978a79-b7e0-4d48-b3a6-22441adcd6a7)


### iv)	Creating the new test cell view

•	Go to CIW window, Execute File-New-Cell view<br>
	Setup the new file form<br>
	Library: Select the one you created.<br>
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test<br>
	View: Schematic<br>
	Type: Schematic press OK<br>
•	Follow the step 3(ii) d to make the required connections<br>

![image](https://github.com/user-attachments/assets/a8204683-5180-4ee5-a6de-89fa7dd3faa3)



 
### Analog simulation by SPECTRE.
•	In test cell view window<br>
•	Launch – ADE L(Analog Design Environment)<br>
	Execute Setup—Simulation/directory/Host A new window opens<br>
	Set the simulation window to spectre and click ok<br>
	Execute Analysis – Choose. A window opens.<br>
	Select the type and set the specifications and press OK<br>
	Execute Output s—to be plotted – Select on Schematic<br>
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse<br>
•	Execute Simulation -- Net list and Run<br>
 
![image](https://github.com/user-attachments/assets/9696aa52-870d-4408-a4f3-081b865b0e26)



For Transient Analysis Settings and Output
 
![image](https://github.com/user-attachments/assets/851fb0ef-a796-4abc-a999-f0928929daef)

![image](https://github.com/user-attachments/assets/d192d3f4-2df3-4110-b7b7-4fa08fc9f0b2)



### Results:
The design and implementation of the D-flip-flop using Cadence EDA tools were successfully completed. The simulated results confirmed the correct operation of the flip-flop, with proper synchronization of the input data with the clock signal. Key performance parameters such as propagation delay, power consumption, and area utilization were evaluated, aligning with expected theoretical values.











