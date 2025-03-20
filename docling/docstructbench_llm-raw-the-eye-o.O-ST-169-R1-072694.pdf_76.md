## Result Parameter Details

## Peripheral Control Status

The SMPC outputs the peripheral control status to the status register (SR) when the SMPC control mode is used. The status register (SR) is a that can be read without regard for the INTBACK command. However; when the register is read when the INTBACK command is not in use, all bits except the RESB bit will undefined. register

Figure 3.13 Peripheral Control Status

<!-- image -->

8