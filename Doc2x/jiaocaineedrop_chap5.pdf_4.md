

![0195428b-eadd-701f-aa59-e05f4010752e_0_179_228_1373_1362_0.jpg](images/0195428b-eadd-701f-aa59-e05f4010752e_0_179_228_1373_1362_0.jpg)

(f) The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).

## Exercise 5.10

We use similar language to that on page 210 , with appropriate modifications:

The SLR(1) parsing algorithm. Let \( s \) be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:

(1) If state \( s \) contains any item of the form \( A \rightarrow  \alpha .{X\beta } \) , where \( X \) is a terminal, and \( X \) is the next token in the input string, then the action is to remove the current input token and push onto the stack the number of the state containing the item \( A \rightarrow  {\alpha X}.\beta \) .