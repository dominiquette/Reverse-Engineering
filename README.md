# Reverse Engineering: FindMe_J Challenge

## Overview
This project involved reverse engineering a compiled Java `.class` file to find a hidden flag. The challenge was completed using bytecode analysis, disassembly, and decompilation techniques.

## Tools Used
- `javap` - Java Bytecode Disassembler  
- `JD-GUI` - Java Decompiler  
- `HxD` - Hex Editor  

## Process  
1. **File Verification:** Checked file type using `file FindMe.class`.  
2. **Bytecode Disassembly:** Used `javap -verbose FindMe.class` to inspect structure.  
3. **Hex Analysis:** Opened the file in `HxD` to find readable strings.  
4. **Decompilation:** Used `JD-GUI` to reconstruct the Java source code.  
5. **Extracting the Flag:** Identified a `charAt()` sequence that built the key.  

## Findings  
- The program checked user input against a predefined key.  
- By reversing the `charAt()` sequence, the flag was found:  
***🚩 VRcG{707_y0u_f0und_M3}***


## References  
- [Java Bytecode Versions](https://javaalmanac.io/bytecode/versions/)  
- [Using javap](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javap.html)  
