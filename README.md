# VSD-Workshop
NASSCOM-VSD SoC Design workshop (22 May 2024 - 5 June 2024)

Day 1: Inception of open-source EDA, OpenLANE and Sky130 PDK

How to invoke OpenLANE flow:
1. First, navigate to the path in the virtual machine: ```Desktop/work/tools/openlane_working_dir/openlane```.
2. Run the command ```docker``` to start the flow.
3. Then use the command ```./flow.tcl -interactive``` to enter OpenLANE in interactive mode.
4. In interactive mode, type ```package require openlane 0.9```.
5. We have decided to run this flow for PicoRV32A, which is a CPU core used to implement the RISC V instruction set.
6. Prepare for synthesis using the command ```prep -design picorv32a ```. Note that these designs are already present in ```~/openlane_working_dir/openlane/designs``` directory.
7. Run synthesis using the command ```run_synthesis```.
8. Navigate to the location ```designs/picorv32a/runs``` and locate the appropriate folder using the date of running the synthesis. Go inside that folder to find the results.
9. Now, the objective of the first day lab session is to find the flip flop ratio.
10. Flip flop ratio is given by
<p align ="center">
  $`F/F ratio =\frac{Number of flip flops}{Number of cells}`$ 
</p>
