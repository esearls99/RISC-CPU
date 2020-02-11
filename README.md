# RISC-CPU
Designed on Circuitverse: https://circuitverse.org/users/11904/projects/51881

This is the current working state of a RISC processor I've been designing since December 2019.
The CPU runs on a subset of the RISC-V instruction set which I wrote myself, all coding was done directly in machine code hard-coded to a ROM. My RISC-V implementation is roughly the same as standard RISC-V excepting a few instructions. See my specications sheet: risc-v.txt
My CPU is capable of basic arithmatic, conditional branching, and load/store functionality. Here is a list of its operations:
      r-types| i-types|b-types|load-store types
      add     addi     beq     lw 
      sub     andi     bne     sw
      and     ori
      or      xori
      xor
      
I apologize for the platform I designed this on; it was were I started and it works. The program I currently have the CPU wired to run is extremly simple. It stores values to registers 1 and 2, using an immediate value and a value stored in memory. Next, it adds the values of these two registers, storing the result in register 3. Then the program enters an infinite loop state, completing the program. See myprogram.txt for exact details. I put a ton of time into this project and what resulted was a terribly slow CPU with extremly limited functionality. I don't think there's much more to be done with this project but I'm very glad that I have something which works.
