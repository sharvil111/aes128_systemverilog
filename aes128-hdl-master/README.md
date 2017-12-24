AES-128
=======

A VHDL and SystemVerilog implementation of the 128-bit version of the [Advanced
Encryption Standard
(AES)](http://csrc.nist.gov/publications/fips/fips197/fips-197.pdf) targeting
high-throughput applications. The example has been developed in order to serve
as an extended example for a VLSI front-end design accompanying the book by
H. Kaeslin entitled [*Top-Down Digital VLSI
Design*](http://store.elsevier.com/product.jsp?isbn=9780128007303).

Summary
-------

Designing and developing a hardware architecture is a complex task. The book [*Top-Down Digital VLSI
Design*](http://store.elsevier.com/product.jsp?isbn=9780128007303) provides all
the information required to succeed with the front-end of a design. However, it
does not offer to space to include a more exhaustive example like this AES
implementation.

This project offers a VHDL and a SystemVerilog implementation of the AES-128
algorithm. It contains synthesizeable RTL code in both languages and provides
simulation and synthesis scripts written in [Tcl](http://www.tcl.tk/). The following
[EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) tools have
been used in order to realize the designs:

- **Simulator:** *Questa Sim 10.3a* by *Mentor Graphics*
- **Synthesizer:** *Design Compiler Version 2013.12* by *Synopsys*

Synthesis results are presented for a mature 65nm CMOS technology by United
Microelectronics Corporation ([UMC](http://www.umc.com/)). We also include a
simple area/time tradeoff for certain timing constraints for different S-box
implementaions as shown in the following image:

![AT plot of AES S-box evaluation](https://github.com/mbgh/aes128-hdl/blob/master/at_plot_sbox_eval.png)

Summarizing, with the present AES-128 front-end design example we demonstrate:

- Functionally identical RTL synthesis models in both VHDL and SystemVerilog
- Architectural tradeoffs and a small selection of optimization techniques
- Timing constraints and their impact on the synthesis outcome (*AT*-plot)
- A self-checking testbench that applies directed and random test suites
- Organizing a verification environment into re-usable modules using UVM
- Co-simulating a VHDL model with a SystemVerilog testbench
- Shell and Tcl scripts for governing simulation and synthesis runs


Documentation
-------------

A more detailed documentation of the AES-128 architecture is available
[here](https://github.com/mbgh/aes128-hdl/blob/master/doc/doc/aes128-doc.pdf). Moreover,
documentations of the synthesizeable
[VHDL](https://mbgh.github.io/aes128-hdl/vhdl/index.html) and the
[SystemVerilog](https://mbgh.github.io/aes128-hdl/sv/index.html) source code
can be obtained. We also provide a brief documentation of the [verification
environment](https://mbgh.github.io/aes128-hdl/tb/index.html) based on
[UVM](https://en.wikipedia.org/wiki/Universal_Verification_Methodology).

