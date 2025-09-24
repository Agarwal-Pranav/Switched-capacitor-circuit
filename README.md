**First Order Switched Capacitor Filter**

This repository contains the design, simulation, and analysis of a First Order Switched Capacitor Filter. Switched capacitor filters are widely used in integrated circuits due to their precision, compact size, and ability to achieve high-performance analog signal processing using only capacitors and switches.

**Overview**

A first order switched capacitor filter is a basic building block for analog signal processing. It replaces resistors with capacitors and switches controlled by a clock, making it suitable for integration in CMOS technology. The cut-off frequency of the filter is determined by the ratio of the capacitors and the clock frequency.

**Circuit Description**

The circuit implements a first-order low-pass filter using two capacitors (C1 and C2) and analog switches driven by a non-overlapping clock. The effective resistance is emulated by the switching action, allowing precise frequency control.

**Key Components:**

Capacitors: C1, C2
Switches: S1, S2 (controlled by clock phases)
Clock: Non-overlapping, two-phase

**How It Works**

Switching Action: The switches alternate between charging C1 from the input and transferring charge to C2.
Filtering: The output across C2 provides a filtered version of the input, based on the clock frequency and capacitor values.
Frequency Control: The cut-off frequency (f_c) is given by:
f_c = f_clk * (C1 / C2) / (2π)
