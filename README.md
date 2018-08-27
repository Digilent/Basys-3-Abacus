Basys 3 Abacus Demo
==============
 
Description
--------------
This project is a Vivado demo using the Basys 3's switches, LEDs, pushbuttons, and seven-segment display, written in Verilog. When programmed onto the board, the Abacus demo can perform one of four arithmetic functions on two 8-bit numbers. Switches 15-8 represent input A and switches 7-0 represent input B. The pushbuttons select between subtraction, multiplication, division, and modulo operations as shown in the table below. The result of the selected operation is displayed on the seven-segment display. Once the operation button is released, the result of the operation scrolls across the seven segment display.
 
| Button | Function               |
| ------ | ---------------------- |
| BTNU   | Subtraction (A-B)      |
| BTND   | Multiplication (A\*B)  |
| BTNR   | Division (A/B)         |
| BTNL   | Modulo/Remainder (A%B) |

Requirements
--------------
* **Basys 3**: To purchase a Basys 3, see the Digilent [Store](https://store.digilentinc.com/basys-3-artix-7-fpga-trainer-board-recommended-for-introductory-users/)
* **Vivado 2018.2 Installation**: To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **MicroUSB Cable**

Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Basys-3-Abacus/releases).
2. Open the project in Vivado 2018.2 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Basys-3-Abacus.xpr".
3. In the Flow Navigator panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug a Basys 3 into the computer using a MicroUSB cable.
5. Open a serial terminal emulator (such as TeraTerm) and connect it to the Basys 3's serial port, using a baud rate of 9600.
6. In the green bar at the top of the Vivado window, click "Open target". Select "Auto connect" from the drop down menu.
7. In the green bar at the top of the Vivado window, click "Program device".
8. In the Program Device Wizard, enter "\<archive extracted location\>vivado_proj/Basys-3-Abacus.runs/impl_1/Basys3_Abacus_Top.bit" into the "Bitstream file" field. Then click **Program**.
9. The demo will now be programmed onto the Basys 3. See the Introduction section of this README for a description of how this demo works.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project.

Check out the Basys 3's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/basys-3/start) to find more documentation, demos, and tutorials.

For technical support or questions, please post on the [Digilent Forum](https://forum.digilentinc.com).

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)
