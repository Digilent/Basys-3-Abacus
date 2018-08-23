Basys 3 Abacus Demo
==============

Introduction
--------------
This project is a Verilog demo using the Basys 3, switches, LEDs, pushbuttons, and seven-segment display. When programmed onto the board, operands are taken from the switches and displayed on the LEDs. The pushbuttons select between subtraction, multiplication, division, and modulo operations and the result of the selected operation is displayed in hexadecimal on the seven segment.
 
| Button | Function         |  
| ------ | ---------------- |
| BTNU   | Subtraction      |
| BTND   | Multiplication   |
| BTNR   | Division         |
| BTNL   | Modulo/Remainder |

| Switches      | Function         |  
| ------------- | ---------------- |
| Switches 15-8 | represent input A|
| Switches 7-0  | represent input B|



Requirements
--------------
* **Basys 3**: To purchase a Basys 3, see the Digilent [Store](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
* **Vivado 2018.2 Installation**: To learn how to get Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **Serial Terminal Emulator**: For more information, see the [Installating and Using a Terminal Emulator Tutorial](https://reference.digilentinc.com/learn/programmable-logic/tutorials/tera-term).
* **MicroUSB Cable**

Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Basys-3-Abacus/releases).
2. Open the project in Vivado 2018.2 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Basys-3-Abacus.xpr".
3. In the *Flow Navigator* panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug a Basys 3 into the computer running Vivado using a MicroUSB cable.
5. Open a serial terminal emulator (such as TeraTerm) and connect it to the Basys 3's serial port, using a baud rate of 9600.
6. Click "Open target" in the green bar at the top of the window. Select "Auto connect" from the drop down menu.
7. Click "Program device" in the green bar at the top of the window. In the "Program Device" Wizard, enter "\<archive extracted location\>vivado_proj/Basys-3-Abacus.runs/impl_1/top.bit" into the "Bitstream file" field. Then click **Program**.
8. The demo will now be programmed onto the Basys 3. See the *Introduction* section of this README for a description of how this demo works.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project. Check out the Basys 3's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/basys-3/start?redirect=1) to find more documentation, demos, and tutorials.

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)
