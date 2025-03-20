|RAW MATERIAL FAMILY|NUMBER OF TINTS|RES (DPI)|FINISHING TYPE|NUMBER OF TOOLS|MACHINE|
|---|---|---|---|---|---|
|FABRIC| |NE| | |830|
|FABRIC| |280|NE| |830|
|FABRIC| |280|NE:| |830|
|FABRIC| |360|NE:| |830|
|FABRIC| |360|NE| |830|
|FABRIC| |400|LAMINATED| |2200|
|FABRIC| |400|LAMINATED| |NILPETER|
|FABRIC| |400|LAMINATED|2|NILPETER|
|FABRIC| |700|NE|2|2200|
|FABRIC| |700|N.E:|2|2200|
|FABRIC| |700|NE:| |2200|
|FABRIC| |800|LAMINATED|2|NILPETER|
|FABRIC| |800|NE|2|NILPETER|
|FABRIC| |800|NE:| |NILPETER|
|CARDBOARD| |280|NE| |830|
|CARDBOARD| |360|NE| |830|
|CARDBOARD|3|360|NE:| |830|
|CARDBOARD| |500|LAMINATED| |2200|
|CARDBOARD| |360|NE;| |2200|
|CARDBOARD|5|600|LAMINATED| |2200|
|CARDBOARD| |700|NE:|3|NILPETER|
|CARDBOARD| |800|NE:| |NILPETER|
|CARDBOARD| |700|LAMINATED| |NILPETER|
|CARDBOARD| |800|LAMINATED| |NILPETER|
|KIMDURA| |360|NE;| |2200|
|KIMDURA| |400|LAMINATED| |2200|
|KIMDURA| |400|LAMINATED| |2200|
|KIMDURA| |400|LAMINATED| |2200|
|KIMDURA| |360|NE.| |NILPETER|
|KIMDURA| |360|NE:| |NILPETER|
|BOPP| |280|NE:| |830|
|BOPP| |360|LAMINATED| |830|
|BOPP| |400|NE:| |2200|
|BOPP| |400|LAMINATED| |2200|
|BOPP| |500|NE.| |2200|
|BOPP| |700|NE:| |2200|
|BOPP| |800|NE:| |NILPETER|
|PAPER| |280|NE:| |830|
|PAPER| |280|NE.| |830|
|PAPER| |360|NE:| |830|
|PAPER| |360|NE| |830|
|PAPER| |500|NE.| |2200|
|PAPER| |600|SULFATED| |2200|
|PAPER| |700|LAMINATED| |2200|
|PAPER|2|600|LAMINATED|2|2200|
|PAPER| |360|LAMINATED| |NILPETER|
|PAPER|5|700|NE:| |NILPETER|
|PAPER| |800|NE| |NILPETER|
|OTHER| |NE:|NE| |2200|
|OTHER|500|NE|3| |NILPETER|

Fig: The training matrix

as input 1 of the training matrix has six different values, six processing units are built: However, the actual value is represented by string, which is not a suitable input type for the FANN. Thus, such values are converted to a stream of 0's and 1's. Table 1 illustrates the codification for the raw material family.

The prior codification is necessary because FANNs only handle values within the closed interval [0,1]. Therefore, the actual input and output values that the net receives and obtains are 0's and 1's. This codification-decoding is done by the encoder class attached to the machine codified in a similar way. Tables 2-6 show the resultant codification:

Consequently, the number of processing units in the input layer of the FANN equals the number of codified input values. For this case, 25 processing units in the input.