# cmpen331-lab-4-solved
**TO GET THIS SOLUTION VISIT:** [CMPEN331 Lab 4 Solved](https://www.ankitcodinghub.com/product/cmpen331-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123465&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMPEN331 Lab 4  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
CMPEN 331 – Computer Organization and Design,

Lab 4

This lab introduces the idea of the pipelining technique for building a fast CPU. The students will obtain experience with the design implementation and testing of the first four stages (Instruction Fetch, Instruction Decode, Instruction Execute, Memory) of the five-stage pipelined CPU using the Xilinx design package for FPGAs. It is assumed that students are familiar with the operation of the Xilinx design package for Field Programmable Gate Arrays (FPGAs) through the Xilinix tutorial available in the class website.

1. Pipelining

As described in lab 4

2. Circuits of the Instruction Fetch Stage

As described in lab 4

3. Circuits of the Instruction Decode Stage

As described in lab 4

4. Circuits of the Execution Stage

Referring to Figure 1, (8.5) in the third cycle the first instruction entered the EXE stage. The ALU performs addition, and the multiplexer selects the immediate. A letter “e” is prefixed to each control signal in order to distinguish it from that in the ID stage. The second instruction is being decoded in the ID stage and the third instruction is being fetched in the IF stage. All the four pipeline registers are updated at the end of the cycle.

5. Circuits of the Memory Access Stage

Referring to Figure 2, (8.6) in the fourth cycle of the first instruction entered the MEM stage. The only task in this stage is to read data memory. All the control signals have a prefix “m”. The second instruction entered the EXE stage; the third instruction is being decoded in the ID stage; and the fourth instruction is being fetched in the IF stage. All the five pipeline registers are updated at the end of the cycle.

Figure 1 Pipeline execution (EXE) stage

Figure 2 Pipeline memory access (MEM) stage

6. Table 1 lists the names and usages of the 32 registers in the register file.

Table 1 MIPS general purpose register

$zero 0 Constant 0

$at 1 Reserved for assembler

$v0, $v1 2, 3 Function return values

$a0 – $a3 4 – 7 Function argument values

$t0 – $t7 8 – 15 Temporary (caller saved)

$s0 – $s7 16 – 23 Temporary (callee saved)

$t8, $t9 24, 25 Temporary (caller saved)

$k0, $k1 26, 27 Reserved for OS Kernel

$gp 28 Pointer to Global Area

$sp 29 Stack Pointer

$fp 30 Frame Pointer

$ra 31 Return Address

7. Table 2 lists some MIPS instructions that will be implemented in our CPU

Table 2 MIPS integration instruction

8. Initialize the first 10 words of the Data memory with the following HEX values:

A00000AA

10000011

20000022

30000033

40000044

50000055

60000066

70000077

80000088

90000099

9. Write a Verilog code that implement the following instructions using the design shown in Figure 2. Write a Verilog test bench to verify your code: (You have to show all the signals written into the MEM/WB register and output from EX/MEM register in your simulation outputs)

instruction comment

lw $2, 00($1) # $2  memory[$1+00]; load x[0] lw $3, 04($1) # $3  memory[$1+04]; load x[1] lw $4, 08($1) # $4  memory[$1+08]; load x[2] lw $5, 12($1) # $5  memory[$1+12]; load x[3]

Assume that register $1 has the value of 0

10. Write a report that contains the following:

a. Your Verilog design code. Use:

i. Device: XC7Z010- -1CLG400C

b. Your Verilog® Test Bench design code. Add “`timescale 1ns/1ps” as the first line of your test bench file.

c. The waveforms resulting from the verification of your design with ModelSim showing all the signals written into the MEM/WB register and output from EX/MEM register.

d. The design schematics from the Xilinx synthesis of your design. Do not use any area constraints. e. Snapshot of the I/O Planning and

f. Snapshot of the floor planning

11. REPORT FORMAT: Free form, but it must be:

g. One report per student.

h. Have a cover sheet with identification: Title, Class, Your Name, etc.

i. Using Microsoft word and it should be uploaded in word format not PDF. If you know LaTex, you should upload the Tex file in addition to the PDF file.

j. Double spaced

12. You have to upload the whole project design file zipped with the word file.
