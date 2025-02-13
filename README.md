# VHDL Signal Assignment Timing Issue

This repository demonstrates a subtle timing issue in VHDL that can lead to unexpected results. The bug involves the incorrect handling of signal assignments within a process, causing data output to be delayed by a clock cycle or be incorrect. 

## Description of the Bug
The `bug.vhdl` file contains a simple entity with an input and output port. The process intends to copy the input data to the output port. However, due to the way signals are updated, the output is not a direct copy in the same clock cycle. The solution showcases the correct implementation.  This example highlights the importance of understanding VHDL's signal update mechanism and how to correctly handle assignments within processes for predictable behavior.

## Solution
The `bugSolution.vhdl` file presents a corrected version of the VHDL code.  The changes address the timing issue resulting in correct output synchronization.