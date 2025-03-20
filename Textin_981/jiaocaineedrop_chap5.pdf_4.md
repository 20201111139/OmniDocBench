(d)


|  | Parsing stack  | Input  | Action  |
| -- | -- | -- | -- |
| 1  | &#36;0 | int x,y,z&#36; | shift 3  |
| 2  | &#36;0int3 | x,y,z&#36; | reduce 2  |
| 3  | &#36;0T2 | x,y,z&#36; | shift 6  |
| 4  | &#36;0T2id6 | ,Y,z&#36; | reduce 5  |
| 5  | &#36;0T2V5 | ,Y,z&#36; | shift 7  |
| 6  | &#36;0T2V5,7 | y,z&#36; | shift 8  |
| 7  | &#36;0T2V5,7id8 | ,z&#36; | reduce 4  |
| 8  | &#36;0T2V5 | ,z&#36; | shift 7  |
| 9  | &#36;0T2V5,7 | z&#36; | shift 8  |
| 10  | &#36;0T2V5,7id8 | &#36; | reduce 4  |
| 11  | &#36;0T2V5 | &#36; | reduce 1  |
| 12  | &#36;OD1 | &#36; | accept  |


(e)

<!-- [D'→.D, &#36;] D [ D ^ { \prime } \rightarrow 0 .,&#36;] [D→ .TV, &#36;] [T →.in t,id] ① [T →.float,id] 0 T D→ T⋅V, [V→⋅V , S ] \\ , i d , S int float [V→⋅/ ② id [T int.,id] [T float.,id] ③ 4 [V→id.,S/,] ⑥ [D→TV,S] [V→V,id,S/, 、 [ V \rightarrow V _ { 1 } \cdot i d , S / , ] id [V→V,id.,S/,] ⑤ ⑦ ⑧  -->
![](https://web-api.textin.com/ocr_image/external/dc5ab46153564bcb.jpg)

(f)The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).

## Exercise 5.10

We use similar language to that on page 210, with appropriate modifications:

The SLR(1) parsing algorithm. Let s be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:

(1) If state s contains any item of the formA→α.Xβ, where Xis a terminal, and Xis the next token in the input string, then the action is to remove the current input token and push onto the stack the number of the state containing the itemA→αX.β.

