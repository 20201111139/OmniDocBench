<table border=1>
<tr>
<td rowspan="2">
<table>
<tr>
<td>RAW MATERIAL</td>
</tr>
<tr>
<td>FAMILY</td>
</tr>
</table>
</td>
<td rowspan="2">
<table>
<tr>
<td>NUMBER</td>
</tr>
<tr>
<td>OF TINTS</td>
</tr>
</table>
</td>
</tr>
</table> & \multicolumn{2}{|c|}{ INPUTS } & \multirow{2}{*}{<table border=1>
<tr>
<td>OUTPUT</td>
</tr>
<tr>
<td>MACHINE</td>
</tr>
<tr>
<td>TOOLS</td>
</tr>
</table> \\
\hline & & & <table border=1>
<tr>
<td>FINISHING</td>
</tr>
<tr>
<td>TYPE</td>
</tr>
</table>& <table border=1>
<tr>
<td>NUMBER OF</td>
</tr>
<tr>
<td>TOOLS</td>
</tr>
</table>& \\
\hline FABRIC & 0 & N.E. & N.E. & 1 & 830 \\
\hline FABRIC & 0 & 280 & N.E. & 1 & 830 \\
\hline FABRIC \(\quad 1\) & 0 & 360 & N.E. & 1 & 830 \\
\hline FABRIC & 2 & 360 & N.E. & 1 & 830 \\
\cline { 2 - 5 } FABRIC & 3 & 360 & N.E. & 1 & 830 \\
\(\quad\) FABRIC & 4 & 360 & LAMINATED & 1 & 830 \\
\hline FABRIC & 3 & 400 & LAMINATED & 2 & NILPETER \\
\hline FABRIC & 3 & 400 & LAMINATE & 2 & NILPETER \\
\hline FABRIC & 4 & 700 & N.E. & 2 & 2200 \\
\hline FABRIC & 4 & 700 & N.E. 2 & 2 & NILPETER \\
\hline FABRIC & 4 & 800 & LAMINATED & 2 & NILPETER \\
\hline FABB & 7 & 800 & N.E. & 2 & NILPETER \\
\hline FABB & 7 & 880 & N.E. & 1 & NILPETER \\
\hline CARDBOARD & 0 & 800 & N.E. 1 & 1 & NILPETER \\
\hline CARDBOARD & 1 & 360 & N.E. 1 & 1 & 830 \\
\hline CARDBOARD & 1 & 360 & N.E 1 & 1 & 830 \\
\hline CARDBOARD & \(4 \quad 500\) & LAMINATED & 1 & 2200 \\
\hline CARDBOARD & \(4 \quad 360\) & N.E. 1 & 1 & 2200 \\
\hline CARDBOARD & \(6 \quad 500\) & N.E. 1 & 1 & 2200 \\
\cline { 2 - 5 } CARDBOARD & \(6 \quad 700\) & N.E. 2 & 1 & 2200 \\
\hline CARDBOARD & \(5 \quad 800\) & N.E. 1 & 1 & 2200 \\
FABRIC & \(6 \quad 800\) & LAMINATED & 1 & 2200 \\
\(\quad\) CARDBOARD & \(5 \quad 800\) & LAMINATED & 2 & NILPETER \\
\hline KIMDURA & 0 & 360 & N.E. 1 & 1 & 2200 \\
\hline KIMDURA & 1 & 400 & LAMINATED & 2 & 2200 \\
\hline KIMDURA & 1 & 100 & LAMINATED & 1 & 2200 \\
\hline KIMDURA & 2 & 400 & LAMINATED & 1 & 2200 \\
\hcline { 2 - 5 } KIMDURA & 6 & 360 & N.E. 1 & 1 & NILPETER \\
\hline BOPP & 0 & 280 & N.E. 1 & 1 & 830 \\
\hline BOPP & 0 & 280 & N.E. & 1 & 835 \\
\hline BOPP & 3 & 400 & N.E. 1 & 1 & 2200 \\
\hcline { 2 - 5 }\) BOPP & 3 & 400 & LAMINATED & 1 & 2200 \(\quad 2\) \\
\hline BOPP & 3 & 400 & LAMINATED & 1 \\
\hline BOPP & 6 & 700 & N.E. 1 & 1 & 2200 \\
\cline { \(\quad 2 - 5}\) BOPP & 7 & 800 & N.E. 2 & 1 & NILPETER \\
\hline BOPP & 6 & 700 & N.E. & 1 & 830 \\
\hline PAPER & 0 & 280 & N.E. 1 & 1 & 1 \\
\hline PAPER & 1 & 360 & N.E. 1 & 1 & 1 \\
\hline PAPER \(\quad 2\) & 3 & 500 & N.E. 1 & 1 & 2200 \\
\(\quad\) PAPER & 3 & 500 & N.E. 1 & 1 & 1 \\
\hline PAPER\(\quad 3\) & 3 & 600 & SULPATED & 2 & 2200 \\
\hline PAPER\(\quad 2\) & 3 & 600 & LAMINATED & 2 & 2200 \\
\hcline { 2 - 5 } PAPER & 3 & 600 & LAMINATED & 2 & 2000 \\
\hline PAPER & 6 & 360 & LAMINATED & 1 & 1 \\
\hline PAPER & 6 & 360 & N.E. 1 & 1 & 1 \\
\cline { 2 - 5 } PAPER & 6 & 800 & N.E. 1 & 1 & 1 \\
\hline OTHER & 0 & N.E. & N.E. & 1 & 2200 \\
\hline OTHER & 4 & 500 & N.E. & 3 & 1 \\
\hline
\end{tabular}
Fig. 2. The training matrix.
as input 1 of the training matrix has six different values, six processing units are built. However, the actual value is represented by a string, which is not a suitable input type for the FANN. Thus, such values are converted to a stream of 0 's and 1'. Table 1 illustrates the codification for the raw material family.
The prior codification is necessary because FANNs only handle values within the closed interval \([0,\). Therefore, the actual input and output values that the net receives and obtains are 0 's and 1'. This codification-decodification is done by the encoder class attached to the machine agent (see Fig. 5). Therefore, the FANN has six processing units in the input layer, which are in charge of dealing exclusively with the raw material family. The totality of discrete values contained in the input and output sets were
Table 1
Codification of the raw material family set
<table border=1>
<tr>
<td>Input stream</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td>Raw material family</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1</td>
<td>0</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1</td>
<td>0</td>
<td>0</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>1</td>
<td>0</td>
<td>0</td>
<td>0</td>
</tr>
<tr>
<td>1</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
</tr>
<tr>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
</tr>
</table>codified in a similar way. Tables 2-6 show the resultant codification.
Consequently, the number of processing units in the input layer of the FANN equals the number of codified input values. For this case, 25 processing units in the input