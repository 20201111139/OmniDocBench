<!-- image -->

|                                              | Parsing stack                                | Action                                       |
|----------------------------------------------|----------------------------------------------|----------------------------------------------|
| 1                                            | $ 0                                          | Ishift 3                                     |
|                                              | $ 0 int 3                                    | reduce 2                                     |
| 3                                            | $ 0 T2                                       | Ishift 6                                     |
| ;                                            | $0 T2 id 6                                   | reduce 5 'Y, 2S                              |
|                                              |                                              | shift 8                                      |
|                                              |                                              | reduce 4                                     |
| 8                                            | $0 T2 V5                                     | shift 7                                      |
| 9                                            |                                              | shift 8                                      |
| 10                                           |                                              | $ reduce 4                                   |
| 11                                           |                                              | reduce 1                                     |
| 12                                           |                                              |                                              |
|                                              |                                              | laccept                                      |
|                                              | [ 9 D , $ ] [D 9 TV , $] [T int float        |                                              |
| [D' = D . , $ ] [T id] [D 9                  | [D' = D . , $ ] [T id] [D 9                  | [D' = D . , $ ] [T id] [D 9                  |
| [V id int float 2 id [T int id [T 9 float id | [V id int float 2 id [T int id [T 9 float id | [V id int float 2 id [T int id [T 9 float id |
| id $/ ,                                      | id $/ ,                                      | id $/ ,                                      |

The LALR(I) parsing table is the same as the SLR(I) parsing table shown in (c)

## Exercise 5.10

We use similar language to that on page 210, with appropriate modifications:

The SLR(I) parsing algorithm. Let s be the current state whose number is at the of the top

a.Xß; where Xis a terminal, and Xis the onto push