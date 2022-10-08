# Design and Implementation of 8 Bit SRAM

## Content
1. Abstact
2. Introduction
3. Decoder
4. 6T SRAM
5. 1 bit SSRAM
6. Results
7. Files
8.  Reference
9. Acknowledgmenet

## Abstract
Static Random Access Memory (SRAM) is a static memory cell which is being used in various electronic devices. It is faster as compared to other memory cells and even consumes lesser power and is not required to be refreshed periodically. The application of this circuit can be a simple memory element, a Lookup table for an FPGA etc.
</br>

## 1.	Introduction
The architecture of the 6T SRAM cell is shown in the figure 1. A basic 6T SRAM cell has two inverters connected back to back.
</br>
We will be using 8 of such circuits in order to get the 8 bits required for the implementation. This array of 1 bit RAM will be modified (read and write) using a decoder circuit. The decoder will be coded in Verilog and the SRAM will be made in Esim.
</br>

## 2.	Decoder and Writer
Decoder is a digital circuit which is used to change a given code into a set of signals. Here we are using a Decoder to select one out of eight 1-bit RAM cells to perform the read/write operation to.
</br>
Decoder
![image](https://github.com/MahimaGoyen/Mixed_signal_design/blob/main/decoder.PNG)
</br>
This circuit provides the input to the 6T SRAM cell. The funtionality of this block is to provide bl and blb to the SRAM cell, when the inputs wl and din are high the bl and blb will also be high else both the outputs will be low. For this design the Writer Circuit has been designed using the NgVeri feature of the eSIM. The Verilog code is as follows:
</br>
Writer
![image](https://github.com/MahimaGoyen/Mixed_signal_design/blob/main/writer.PNG)
</br>
## 3. 6T SRAM
![image](https://github.com/MahimaGoyen/Mixed_signal_design/blob/main/6t.PNG)
</br>
## 4.	1 bit SRAM
![image](https://github.com/MahimaGoyen/Mixed_signal_design/blob/main/1bit.PNG)
</br>
## 5.	8 bit SRAM
![image](https://github.com/MahimaGoyen/Mixed_signal_design/blob/main/8bit.PNG)
</br>

## Acknowlegdements
1. FOSSEE, IIT Bombay
2. Steve Hoover, Founder, Redwood EDA
3. Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd. - kunalpghosh@gmail.com
4. Sumanto Kar, eSim Team, FOSSEE

## Reference
[1] Design of Read and Write Operations for 6t Sram Cell (https://www.iosjournals.org/iosr-jvlsi/papers/vol8-issue1/Version-1/E0801014346.pdf)
[2] “6T SRAM Cell: Design and Analysis” Int. Journal of Engineering Research and Applications, Vol. 4, Issue 3, March 2014 (https://www.ijera.com/papers/Vol4_issue3/Version%201/CX4301574577.pdf)</br>
[3] Sah, Rohit & Hussain, Inamul & Kumar, Manish. (2020). Performance Analysis of a 6T SRAM Cell in 180nm CMOS Technology. 10.9790/4200-05212022.
