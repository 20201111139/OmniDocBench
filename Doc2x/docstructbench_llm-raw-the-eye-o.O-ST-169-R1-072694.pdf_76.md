## Result Parameter Details

## Peripheral Control Status

The SMPC outputs the peripheral control status to the status register (SR) when the SMPC control mode is used. The status register (SR) is a register that can be read without regard for the INTBACK command. However, when the register is read when the INTBACK command is not in use, all bits except the RESB bit will be undefined.

---

	<img src="https://cdn.noedgeai.com/0195421f-3cc9-731a-9884-f948c6789943_0.jpg?x=153&y=550&w=1341&h=954"/>

---

Figure 3.13 Peripheral Control Status