# Compiler Construction: Principles and Practice

# Chapter 5 Exercise Answers

# Page 5

|Parsing stack|Input|Action| |
|---|---|---|---|
|$ 0|int x,Y,2$|shift 3| |
|2 $ 0 int|3|x,Y,28|(reduce 2)|
|3 $ 0 T2|X,Y,25|shift 6| |
|$ 0 T2 id|6|'Y,28|(reduce 5)|
|5 $ 0 T2 V5|'Y,25|shift 7| |
|$ 0 T2 V5,7|Y,28|shift &| |
|$ 0 T2 V5,7 id|8|28|(reduce 4)|
|$ 0 T2 V5|25|shift 7| |
|10 $ 0 T2 V5,7|28|shift 8 0| |
|$ 0 T2 V5,7 id|8|S|(reduce 4)|
|12 $ 0 T2 V5|S|(reduce)| |
|$ 0 D 1| |accept| |
|[D' 7 .D , $1|[D'|0| |
|[T|.TV| | |
|int id| |float id| |
| |[D|T .V , S]| |
| |[V _ V _ id S/, ]| | |
|int|float| | |
|AOU|id| | |
|int. id|~float id| | |
| |id., Sl,| | |
|d>|7TV|S ]| |
| |id,Sl , id| | |
|V.id|Sf_|V -V,|V,id.|

The LALR(1) parsing table is the same as the SLR(1) parsing table shown in (c).

# Exercise 5-10

We use similar language to that on page 210, with appropriate modifications:

The SLR(I) parsing algorithm. Let $ be the current state whose number is at the top of the parsing stack. Then actions are defined as follows:

1. If state $ contains any item of the form A - &.X 8, where X is a terminal, and X is the next token in the input string, then the action is to remove the current input token and pushₒₙₜₒ the stack the number of the state containing the item A -> &X: B.