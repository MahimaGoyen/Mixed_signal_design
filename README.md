# Design and Implementation of 8 Bit SRAM

## Abstract- Static Random Access Memory (SRAM) is a static memory cell which is being used in various electronic devices. It is faster as compared to other memory cells and even consumes lesser power and is not required to be refreshed periodically. The application of this circuit can be a simple memory element, a Lookup table for an FPGA etc.


## 1.	Introduction
The architecture of the 6T SRAM cell is shown in the figure 1. A basic 6T SRAM cell has two inverters connected back to back.

We will be using 8 of such circuits in order to get the 8 bits required for the implementation. This array of 1 bit RAM will be modified (read and write) using a decoder circuit. The decoder will be coded in Verilog and the SRAM will be made in Esim.
##2. Decoder
##3. 6T SRAM Cell
##4. 1bit SRAM
##5. 8NIT SRAM

## Acknowlegdements
1. FOSSEE, IIT Bombay
2. Steve Hoover, Founder, Redwood EDA
3. Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd. - kunalpghosh@gmail.com
4. Sumanto Kar, eSim Team, FOSSEE

##References
[1] Design of Read and Write Operations for 6t Sram Cell (https://www.iosjournals.org/iosr-jvlsi/papers/vol8-issue1/Version-1/E0801014346.pdf)
[2] “6T SRAM Cell: Design and Analysis” Int. Journal of Engineering Research and Applications, Vol. 4, Issue 3, March 2014 (https://www.ijera.com/papers/Vol4_issue3/Version%201/CX4301574577.pdf)
[3] Sah, Rohit & Hussain, Inamul & Kumar, Manish. (2020). Performance Analysis of a 6T SRAM Cell in 180nm CMOS Technology. 10.9790/4200-05212022.
