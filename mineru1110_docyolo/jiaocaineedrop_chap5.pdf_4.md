<td><table  border="1"><thead><tr><td></td><td><b>Parsing stack</b></td><td><b>Input</b></td><td><b>Action</b></td></tr></thead><tbody><tr><td>1</td><td>$0</td><td>int x,y,z$</td><td>shift 3</td></tr><tr><td>2</td><td>$0int3</td><td>x,y,z$</td><td>reduce2</td></tr><tr><td>3</td><td>$OT2</td><td>x,y,z$</td><td>shift 6</td></tr><tr><td>4</td><td>$0T2id6</td><td>,y,z$</td><td>reduce5</td></tr><tr><td>5</td><td>$0T2V5</td><td>,y,z$</td><td>shift 7</td></tr><tr><td>6</td><td>$0T2V5,7</td><td>y,z$</td><td>shift 8</td></tr><tr><td>7</td><td>$0T2V5,7id8</td><td>,2$</td><td>reduce 4</td></tr><tr><td>8</td><td>$0T2V5</td><td>,2$</td><td>shift 7</td></tr><tr><td>9</td><td>$0T2V5,7</td><td>z$</td><td>shift 8</td></tr><tr><td>10</td><td>$0T2V5,7id8</td><td>$</td><td>reduce 4</td></tr><tr><td>11</td><td>$0T2V5</td><td>$</td><td>reduce 1</td></tr><tr><td>12</td><td>$0D1</td><td>S</td><td>accept</td></tr></tbody></table></td>  

(e)  

![](images/ef98ab51c963b539d819f0d8ecbff705993c70184fdb5f1096855e486589504f.jpg)  

(f) The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).  

# Exercise 5.10  

We use similar language to that on page 210, with appropriate modifications:  

The SLR(l) parsing algorithm. Let  $S$  be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:  

(1) If state  $\boldsymbol{S}$  contains any item of the form  $A\to\upalpha\,.X\,\upbeta$  ,where  $X$  is a terminal, and  $\boldsymbol{X}$  is the next token in the input string, then the action is to remove the current input token and push onto the stack the number of the state containing the item  $A\rightarrow\alpha X.\beta$  