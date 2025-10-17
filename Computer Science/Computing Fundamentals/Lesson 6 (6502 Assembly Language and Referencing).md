Here, you worked with a 6502 microprocessor simulator in your browser. The file is on brightspace, in computer fundamentals, week 2, lab, lab week 15.

The 6502 has 6 registers, 4 of which are directly usable by the programmer. Namely:

**The accumulator** (8 bits, represented by A) which is used for arithmetic and logical operations (not including increments and decrements). Data needs to be loaded here before it can be manipulated.

**Index Register X** (8 bits, represented by X) and **Index Register Y** (8 bits, represented by Y) both holdcounters or offsets for accessing memory. Contents can be compared with memory locations and incremented and decremented.

**Flags Register** (8 bits, also known as the status register) indicates the results of an operation. Each bit in the register signifies a different condition, being:

Carry Flag (C), which sets the result to 1 if the previous result caused an overflow. 

Zero Flag (Z), which sets the result to 1 if the previous result was 0.

Negative Flag (N), which sets the result to 1 if the previous result was negative.

==THINGS TO REMEMBER WHEN PROGRAMMING IN ASSEMBLY CODE==

A # signifies that the number is a data value, not a memory address.
A $ means the number is hexadecimal. 
A ; is treated as a comment.

Functions work basically the same as every other programming language. In assembly, you type the name of the function and then add a colon, without needing to add any objects or whatnot. Here's an example function:

lab01:
	LDX #$00

**LD means LoaD**. For example, LDX would mean loading something into the Index Register X. LDA would mean loading something into the accumulator.

**ST means STore.** For example, STA would store a value into the accumulator. (The correct syntax is STA (memory address), (value you want stored.)) Example: STA $0200, X would store the value of X at memory address $0200.

**IN means INcrement**. Example: INX would increment the value stored in the Index Register X by one.

**DE means DEcrement**. Example: DEX would decrement the value stored in the Index Register X by one. 

**CP means ComPare**. In reality, it subtracts one value to another, and it if equals 0, it sets the zero flag (Look up to remember the flags!) to one. 

For example: Say you have a value of FF (256) stored in the X register. If you do CPX #$FF (# = value, not address, $ = hexadecimal value, which means FF means 256), CP would subtract FF from FF (256-256) and would result in 0. This sets the zero flag to one. 

**BEQ means Branch if EQual to zero**. I know. Confusing. These can only be used to run other functions. 

Let's say you had a function that had the CP command from above. If it flips the zero flag to one, nothing actually happens. This is where BEQ comes in. You can use it to check if the zero flag is set to one, and make something happen. 

Assume the zero flag was set to 1. Also assume we have functions lab01 and lab02. Running BEQ lab02 inside of lab01 would make the program jump to function lab02. 

**JMP means JuMP**. Think of it as an else that you would use in an if statement. You can only use it to jump to other functions, which is how looping works. 

At the end of function lab01, you could run JMP lab01 to go back to the start of that loop. 

**BRK means BReaK**. It stops the program. 