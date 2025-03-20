Result Parameter Details

Peripheral Control Status

The SMPC outputs the peripheral control status to the status register (SR) when the SMPC control mode is used. The status register (SR) is a register that can be read without regard for the INTBACK command. However, when the register is read when the INTBACK command is not in use, all bits except the RESB bit will be undefined.

<table>
  <tr>
    <td>SR</td>
    <td>bit7</td>
    <td>bit0</td>
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
  <tr>
    <td>P1MD: Port 1 Mode</td>
  </tr>
  <tr>
    <td>00: 15-byte mode (Returns peripheral data up to a maximum of 15 bytes.)</td>
  </tr>
  <tr>
    <td>01: 255-byte mode (Returns peripheral data up to a maximum of 255 bytes.)</td>
  </tr>
  <tr>
    <td>10: Unused</td>
  </tr>
  <tr>
    <td>11: 0-byte mode (Port is not accessed.)</td>
  </tr>
  <tr>
    <td>P2MD: Port 2 Mode</td>
  </tr>
  <tr>
    <td>00: 15-byte mode (Returns peripheral data up to a maximum of 15 bytes.)</td>
  </tr>
  <tr>
    <td>01: 255-byte mode (Returns peripheral data up to a maximum of 255 bytes.)</td>
  </tr>
  <tr>
    <td>10: Unused</td>
  </tr>
  <tr>
    <td>11: 0-byte mode (Port is not accessed.)</td>
  </tr>
  <tr>
    <td>RESB: Reset Button Status Bit</td>
  </tr>
  <tr>
    <td>0: Reset Button OFF</td>
  </tr>
  <tr>
    <td>1: Reset Button ON</td>
  </tr>
  <tr>
    <td>Reading without regard for INTBACK command is possible. (Shows status for each V-BLANK-IN.)</td>
  </tr>
  <tr>
    <td>NPE: Remaining Peripheral Existence Bit</td>
  </tr>
  <tr>
    <td>0: No remaining data</td>
  </tr>
  <tr>
    <td>1: Remaining data</td>
  </tr>
  <tr>
    <td>PDL: Peripheral Data Location Bit</td>
  </tr>
  <tr>
    <td>0: 2nd or above peripheral data</td>
  </tr>
  <tr>
    <td>1: 1st peripheral data</td>
  </tr>
  <tr>
    <td>bit7: Always 1</td>
  </tr>
</table>

Figure 3.13 Peripheral Control Status