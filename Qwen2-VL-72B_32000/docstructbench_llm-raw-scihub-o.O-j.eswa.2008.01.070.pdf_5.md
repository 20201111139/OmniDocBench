```markdown
\begin{figure}[h]
\centering
\includegraphics[width=0.7\textwidth]{training_matrix.png}
\caption{The training matrix.}
\label{fig:training_matrix}
\end{figure}

as input 1 of the training matrix has six different values, six processing units are built. However, the actual value is represented by a string, which is not a suitable input type for the FANN. Thus, such values are converted to a stream of 0's and 1's. Table 1 illustrates the codification for the raw material family.

The prior codification is necessary because FANNs only handle values within the closed interval [0,1]. Therefore, the actual input and output values that the net receives and obtains are 0's and 1's. This codification-decodification is done by the encoder class attached to the machine agent (see Fig. 5). Therefore, the FANN has six processing units in the input layer, which are in charge of dealing exclusively with the raw material family. The totality of discrete values contained in the input and output sets were codified in a similar way. Tables 2-6 show the resultant codification.

Consequently, the number of processing units in the input layer of the FANN equals the number of codified input values. For this case, 25 processing units in the input

\begin{table}[h]
\centering
\caption{Codification of the raw material family set}
\label{tab:codification}
\begin{tabular}{|c|c|c|c|c|c|c|}
\hline
Input stream & \multicolumn{6}{c|}{Raw material family} \\
\hline
0 & 0 & 0 & 0 & 0 & 1 & Paper \\
0 & 0 & 0 & 0 & 1 & 0 & Fabric \\
0 & 0 & 0 & 1 & 0 & 0 & Kimdura \\
0 & 0 & 1 & 0 & 0 & 0 & Cardboard \\
0 & 1 & 0 & 0 & 0 & 0 & BOPP \\
1 & 0 & 0 & 0 & 0 & 0 & Other \\
\hline
\end{tabular}
\end{table}
```