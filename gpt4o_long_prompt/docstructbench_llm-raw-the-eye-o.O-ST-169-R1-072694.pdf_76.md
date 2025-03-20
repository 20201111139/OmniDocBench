```markdown
## Result Parameter Details

### Peripheral Control Status

The SMPC outputs the peripheral control status to the status register (SR) when the SMPC control mode is used. The status register (SR) is a register that can be read without regard for the INTBACK command. However, when the register is read when the INTBACK command is not in use, all bits except the RESB bit will be undefined.

<table>
<tr>
    <th>SR</th>
    <th>bit7</th>
    <th>bit0</th>
</tr>
<tr>
    <td>1</td>
    <td>PDL</td>
    <td>NPE</td>
    <td>RESB</td>
    <td>P2MD1</td>
    <td>P2MD0</td>
    <td>P1MD1</td>
    <td>P1MD0</td>
</tr>
</table>

**P1MD**: Port 1 Mode  
00: 15-byte mode (Returns peripheral data up to a maximum of 15 bytes.)  
01: 255-byte mode (Returns peripheral data up to a maximum of 255 bytes.)  
10: Unused  
11: 0-byte mode (Port is not accessed.)

**P2MD**: Port 2 Mode  
00: 15-byte mode (Returns peripheral data up to a maximum of 15 bytes.)  
01: 255-byte mode (Returns peripheral data up to a maximum of 255 bytes.)  
10: Unused  
11: 0-byte mode (Port is not accessed.)

**RESB**: Reset Button Status Bit  
0: Reset Button OFF  
1: Reset Button ON  
Reading without regard for INTBACK command is possible. (Shows status for each V-BLANK-IN.)

**NPE**: Remaining Peripheral Existence Bit  
0: No remaining data  
1: Remaining data

**PDL**: Peripheral Data Location Bit  
0: 2nd or above peripheral data  
1: 1st peripheral data

**bit7**: Always 1

**Figure 3.13** Peripheral Control Status
```