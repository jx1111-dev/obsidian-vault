Definitions:
Electric current is a flow of electric charge.

Electronic circuit is a structure that directs and controls electric currents, to perform useful actions.

An integrated circuit is a set of electronic circuits on one small flat piece (called "chip") of semiconductor material, usually silicon. Examples: monolithic integrated circuit, IC, chip, microchip.

A Microprocessor is responsible for executing a sequence of instructions. It operates on numbers and symbols represented in the binary numeral system.

==COMPONENTS OF MICROPROCESSORS==
![[Pasted image 20251007092204.png]]
Central Processing Unit (CPU):
Consists of one or more arithmetic logic units (ALU), registers, and control units.

Registers are used to execute instructions and to store the address or data while running the program.

ALU computes all arithmetic as well as logic operations on data.

It contains:
Inpout and output data,
Input and output status,
Opcode (operation code)
![[Pasted image 20251007092432.png]]
![[Pasted image 20251007092506.png]]
![[Pasted image 20251007092519.png]]
![[Pasted image 20251007092626.png]]

The Control Unit retrieves instruction codes from memory and initiates the sequence of operations required for the ALU.

The computer instruction operation cycle, AKA instruction cycle, is a fetch-decode-execute cycle. It is the basic operational process of a computer. As stated earlier, it consists of:

Fetch: Retrieve a program instruction from its memory.

Decode: Determine what actions the instruction dictates.

Execute: Carry out the action. 

![[Pasted image 20251007092841.png]]
![[Pasted image 20251007092854.png]]

Pipe-lining is a process that allows multiple actions to happen in a single clock. Here is how it works:
![[Pasted image 20251007093003.png]]
As you can see, instead of waiting for one whole cycle to finish, it waits for the clock to be freed up and starts another cycle. This is a lot more efficient. The """"official"""" term for this is concurrency.
It increases the number of instructions that can be executed in a unit of time.

The computer's memory holds the program as well as the data (based on Von neuman architecture)

It is divided into primary memory (ROM (Read Only Memory) and RAM (Random Access Memory))
and secondary memory (external devices, e.g. USBs, external harddrives etc etc.)

The system bus connects units to allow the exchange of information. It consists of data, addresses and control buses to correctly perform data exchange.

The input/output (I/O) interfaces the I/O peripheral devices (mouse, keyboard etc.) to the microprocessor for accepting and sending information.

==ASSEMBLY LANGUAGE==

Before you get into the gutty works of PC language, languages are divided into 2 sections:

High level programs, are more similar to human language, using natural language elements. This makes it easier for humans to read, write and maintain. However, the drawback is that it needs to be translated into machine language by a compiler (compiles entire code at once) or interpreter (compiles code line by line).
Some examples of both are c++ (compiled) and python (can be both, but mostly interpreted.)

Low level programs are closer to binary, which makes them harder to write, read and maintain, unless you are an absolute nerd. 

Commands map closely to processor instructions, which makes them much faster than high level languages.

It is also pretty non-portable because every processor model is different and programs you write for one won't work for others.

Examples: Machine code/Assembly

==Assembly language== is a low-level programming language, and just refers to the language specific to whatever computer part you're programming. It is also called symbolic machine code.

It is the lowest level of abstraction where code is still human readable. 
Example in hex:

a9 80 85 01 65 01

vs. assembly language

LDA #$80
STA $01
ADC $01

Assembly language translates into hex (bytes) which are executed by the processor.

Let's look over an example. This is the MOS 6502 microprocessor. It was manufactured by MOS Technology in the late 1970s. It was used in technological landmarks such as the Apple II, NES, BBC model B, atari 800 and the Commodore 64.

It has a simple instruction set by modern standards, making it cheap to produce.

useful as a case study to learn the principles of low level language programming and processor architecture.

Addresses are locations in computer components, basically.

A 16 bit Address bus:

0000000000000000 to 1111111111111111

Represented as (in hex):

$0000 to $FFFF

Therefore, it has a capacity of 64KB.


![[Pasted image 20251007094841.png]]
![[Pasted image 20251007094857.png]]
![[Pasted image 20251007094907.png]]![[Pasted image 20251007094919.png]