<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works
The proposed project is an 8-bit comparator designed using Verilog for the Tiny Tapeout platform. The main function of this project is to compare two 8-bit input values and generate an output based on their relationship. The first input is provided through ui_in[7:0] and the second input is provided through uio_in[7:0]. The comparator checks whether both inputs are equal, greater than, or less than each other. If both inputs are equal, the output uo_out becomes 1. If the first input is greater than the second input, the output becomes 2. If the first input is less than the second input, the output becomes 4. This project is a combinational circuit, meaning the output changes immediately whenever the input changes, without requiring a clock signal. The bidirectional pins are used only as additional input pins, while the output enable pins are disabled. This design is simple, compact, and suitable for beginners learning digital design and Tiny Tapeout project implementation.

## How to test

To use the 8-bit comparator project, two 8-bit binary numbers must be applied to the input ports ui_in and uio_in. The comparator continuously compares these two input values and produces an output on uo_out. If both inputs are equal, the output becomes decimal 1. If the value applied to ui_in is greater than the value applied to uio_in, the output becomes decimal 2. If the value applied to ui_in is smaller than the value applied to uio_in, the output becomes decimal 4. Since the design is combinational, the output changes immediately whenever the inputs change, without waiting for a clock signal. For example, if ui_in = 10 and uio_in = 3, the output will be 2, indicating that the first input is greater. Similarly, if both inputs are 5, the output becomes 1, indicating equality. This project can be simulated using the provided testbench or implemented on the Tiny Tapeout platform for hardware verification.

## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
