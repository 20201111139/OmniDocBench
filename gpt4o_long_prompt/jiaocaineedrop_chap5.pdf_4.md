```markdown
# Compiler Construction: Principles and Practice  
## Chapter 5 Exercise Answers, Page 5

### (d)

<table>
  <tr>
    <th>Parsing stack</th>
    <th>Input</th>
    <th>Action</th>
  </tr>
  <tr>
    <td>1 S 0</td>
    <td>int x,y,z$</td>
    <td>shift 3</td>
  </tr>
  <tr>
    <td>2 S 0 int 3</td>
    <td>x,y,z$</td>
    <td>reduce 2</td>
  </tr>
  <tr>
    <td>3 S 0 T 2</td>
    <td>x,y,z$</td>
    <td>shift 6</td>
  </tr>
  <tr>
    <td>4 S 0 T 2 id 6</td>
    <td>,y,z$</td>
    <td>reduce 5</td>
  </tr>
  <tr>
    <td>5 S 0 T 2 V 5</td>
    <td>,y,z$</td>
    <td>shift 7</td>
  </tr>
  <tr>
    <td>6 S 0 T 2 V 5,7</td>
    <td>y,z$</td>
    <td>shift 8</td>
  </tr>
  <tr>
    <td>7 S 0 T 2 V 5,7 id 8</td>
    <td>,z$</td>
    <td>reduce 4</td>
  </tr>
  <tr>
    <td>8 S 0 T 2 V 5</td>
    <td>,z$</td>
    <td>shift 7</td>
  </tr>
  <tr>
    <td>9 S 0 T 2 V 5,7</td>
    <td>z$</td>
    <td>shift 8</td>
  </tr>
  <tr>
    <td>10 S 0 T 2 V 5,7 id 8</td>
    <td>$</td>
    <td>reduce 4</td>
  </tr>
  <tr>
    <td>11 S 0 T 2 V 5</td>
    <td>$</td>
    <td>reduce 1</td>
  </tr>
  <tr>
    <td>12 S 0 D 1</td>
    <td>$</td>
    <td>accept</td>
  </tr>
</table>

### (f)

The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).

### Exercise 5.10

We use similar language to that on page 210, with appropriate modifications:

**The SLR(1) parsing algorithm.** Let \( s \) be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:

(1) If state \( s \) contains any item of the form \( A \to \alpha \cdot X \beta \), where \( X \) is a terminal, and \( X \) is the next token in the input string, then the action is to remove the current input token and push onto the stack the number of the state containing the item \( A \to \alpha X \cdot \beta \).
```