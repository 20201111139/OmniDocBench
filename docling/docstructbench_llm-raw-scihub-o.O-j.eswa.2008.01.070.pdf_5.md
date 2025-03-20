Fig. 2

|                 | INPUTS          | INPUTS    |                     |                 | OUTPUT   |
|-----------------|-----------------|-----------|---------------------|-----------------|----------|
| RAW MATERIAL    | NUMBER OF TINTS | RES (DPI) | FINISHING TYPE      | NUMBER OF TOOLS | MACHINE  |
| FAMILY FABRIC   |                 | NE        | NE                  |                 | 830      |
| FABRIC          |                 | 280       | NE                  |                 | 830      |
| FABRIC          |                 | 280       | NE                  |                 | 830      |
| FABRIC          | 2               | 360       | NE                  |                 | 830      |
| FABRIC          |                 | 360       | NE                  |                 | 830      |
| FABRIC          |                 |           | LAMINATED           |                 |          |
|                 | 3               | 400       |                     |                 | 2200     |
| FABRIC          |                 | 400       | LAMINATED           | 2               | NILPETER |
| FABRIC          |                 | 400       | LAMINATED           | 2               | NILPETER |
| FABRIC          |                 | 700       | NE                  |                 | 2200     |
| FABRIC          |                 | 700       | NE                  |                 | 2200     |
| FABRIC          |                 | 700       | NE                  | 2               | 2200     |
| FABRIC          |                 | 800       | LAMINATED           | 2               | NILPETER |
| FABRIC          |                 | 800       | NE                  |                 | NILPETER |
| FABRIC          | 7               | 800       | NE                  |                 | NILPETER |
| CARDBOARD       |                 | 280       | NE                  |                 | 830      |
| CARDBOARD       |                 | 360       | NE                  |                 | 830      |
| CARDBOARD       | 3               | 360       | NE                  |                 | 830      |
| CARDBOARD       |                 | 500       | LAMINATED           |                 | 2200     |
| CARDBOARD       |                 | 360       | NE                  |                 |          |
| CARDBOARD       | 5               | 600       | LAMINATED           |                 | 2200     |
| CARDBOARD       | 6               | 700       | NE                  | 2               | NILPETER |
| CARDBOARD       |                 | 800       | NE                  |                 | NILPETER |
| CARDBOARD       |                 | 700       | LAMINATED           |                 | NILPETER |
| CARDBOARD       | 5               | 800       | LAMINATED           | 2               | NILPETER |
| KIMDURA         |                 | 360       | NE                  |                 | 2200     |
| KIMDURA         |                 | 400       | LAMINATED           |                 | 2200     |
| KIMDURA KIMDURA |                 | 400       | LAMINATED LAMINATED | 2               | 2200     |
| KIMDURA         | 5               | 400 360   | NE                  |                 | 2200     |
|                 |                 |           |                     |                 | NILPETER |
| KIMDURA         |                 | 360       | NE                  |                 | NILPETER |
| BOPP            |                 | 280       | NE                  |                 | 830      |
| BOPP            |                 | 360       | LAMINATED           |                 |          |
| BOPP            | 3               | 400       | NE                  |                 | 2200     |
| BOPP            | 3               | 400       | LAMINATED           |                 | 2200     |
| BOPP            |                 | 500       | NE                  |                 | 2200     |
| BOPP            |                 | 700       | NE                  |                 | 2200     |
| BOPP            |                 | 800       | NE                  |                 | NILPETER |
| PAPER           |                 | 280       | NE                  |                 | 830      |
| PAPER           |                 | 280       | NE                  |                 | 830      |
| PAPER           |                 | 360       | NE                  |                 | 830      |
| PAPER           | 2               | 360       | NE                  |                 | 830      |
| PAPER           | 3               | 500       | NE                  |                 | 2200     |
| PAPER           | 3               | 600       |                     |                 | 2200     |
| PAPER           |                 | 700       | LAMINATED           |                 | 2200     |
| PAPER           |                 | 600       | LAMINATED           | 2               | 2200     |
| PAPER           | 6               | 360       | LAMINATED           |                 | NILPETER |
| PAPER           | 5               | 700       | NE                  | 2               | NILPETER |
| PAPER           | 6               | 800       | NE                  | 3               | NILPETER |
| OTHER           | 0               | NE        | NE                  |                 | 2200     |
| OTHER           |                 | 500       | NE                  |                 | NILPETER |

as processing units are built. However, the actual value is represented by a string, which is not a suitable input type for the FANN. Thus, such values are converted to a stream of 0s and 1s\_ Table 1 illustrates the codification for the raw material family .

The codification is necessary because FANNs only handle   values within the closed interval [0, 1]   Therefore, and obtains are 0s and 1s. This codification-decodifica tion is done by the encoder class attached to the machine agent (see Fig. 5). Therefore, the FANN has six processing units in the input which are in of dealing were prior charge

Table

| Input stream   | Input stream   | Raw material family   |
|----------------|----------------|-----------------------|
|                | 0              | Paper                 |
|                | 0              | Fabric                |
|                |                | Kimdura               |
|                | 0              | Cardboard             |
|                |                | BOPP                  |
|                |                | Other                 |

codified in Tables 2-6 show the resultant codification.

Consequently, the number input of the FANN equals the number of codified input values For this case, 25 processing units in the input layer