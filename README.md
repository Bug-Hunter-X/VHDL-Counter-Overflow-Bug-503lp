# VHDL Counter Overflow Bug

This repository demonstrates a subtle overflow bug in a VHDL counter. The `buggy_counter.vhdl` file contains a counter that increments on each rising clock edge.  The counter uses an integer type with a limited range (0 to 15).  When the counter reaches its maximum value (15), incrementing it causes an overflow, wrapping the counter back to 0. This behavior might be unexpected and can lead to errors in a larger design.

The `fixed_counter.vhdl` file provides a corrected version that prevents overflow by using a modulo operator.