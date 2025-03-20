(d)

(e)

| Parsing stack | Input | Action |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- |
| $ 0 | shift 3 | 1 | int x,y,z5 | 2 | reduce 2 | $ 0 int 3 | x,y,z5 |
| 3 | $072 | shift 6 | x,y,zb | 4 | $0T2id6 | reduce 5 | , V, ZD |
| 5 | $0T2V5 | shift 7 | , y, zb | б | $0T2V5,7 | shift 8 | y,zS |
| 7 | $ 0 T 2 V 5, 7 id 8 | reduce 4 | , z $ | 8 | $ 0 T 2 V 5 | shift 7 | , z $ |
| 9 | $0T2V5,7 | z S | shift 8 | 10 | $ 0 T 2 V 5, 7 id 8 | S | reduce 4 |
| $0 T2 V 5 | S | reduce 1 | l 1 | 6 | 12 | $0D1 | accept |
| D | [D' > D . . $ ] | [D' > . D , $ ] | [D -> . TV , $] |  |  |  |  |
| 1 | [T -> . int, id ] |  |  |  |  |  |  |
| [T -> . float . id ] | T | [D -> T . V , $ ] | 0 |  |  |  |  |
| [V -> . V , id , $/, | [V -> . id , $ /, ] |  |  |  |  |  |  |
| 2 | float | int |  |  |  |  |  |
| id | ->float. id ] | → int. id | [T | IT |  |  |  |
| ( | C |  |  |  |  |  |  |

![](_page_0_Figure_4.jpeg)

(f) The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).

## Exercise 5.10

We use similar language to that on page 210, with appropriate modifications:

The SLR(1) parsing algorithm. Let s be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:

(1) If state s contains any item of the form A -> o. X B, where X is a terminal, and X is the next token in the input string, then the action is to remove the current input token and push onto the stack the number of the state containing the item A -> aX. B.

