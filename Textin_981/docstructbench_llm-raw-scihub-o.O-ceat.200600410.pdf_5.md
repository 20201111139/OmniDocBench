Table 1. Considered process variables of the FCCU case study.


| Variable  | Description  |
| -- | -- |
| 1  | Flow of wash oil to reactor riser  |
| 2  | Flow of fresh feed to reactor riser  |
| 3  | Flow of slurry to reactor riser  |
| 4  | Temperature of fresh feed entering furnace  |
| 5  | Fresh feed temperature to riser  |
| 6  | Furnace firebox temperature  |
| 7  | Combustion air blower inlet suction flow  |
| 8  | Combustion air blower throughput  |
| 9  | Combustion air flow rate  |
| 10  | Lift air blower suction flow  |
| 11  | Lift air blower speed  |
| 12  | Lift air blower throughput  |
| 13  | Riser temperature  |
| 14  | Wet gas compressor suction pressure  |
| 15  | Wet gas compressor inlet suction flow  |
| 16  | Wet gas flow to vapor recovery unit  |
| 17  | Regenerator bed temperature  |
| 18  | Stack gas valve position  |
| 19  | Regenerator pressure  |
| 20  | Standpipe catalys level  |
| 21  | Stack gas$O_{2}$concentration  |
| 22  | Combustion air blower discharge pressure  |
| 23  | Wet gas composition suction valve position  |


<!-- 124 normal * fault1 123 fault2 UoIoeip eJnieel AeuSiL PuodeS fault3 122 121 120 119 118 * 117 81 82 83 84 85 86 87 88 89 90 First Fisher feature direction  -->
![](https://web-api.textin.com/ocr_image/external/b02555527200e15d.jpg)

Figure 2. Scatter plot in original feature space.

<!-- 4 normal 3.8 * fault1 LoIeIp eJneel eusIL IeuJex puooeS fault2 3.6 fault3 3.4 3.2 3 2.8 2.6 2.4 104 106 108 110 112 First kernel Fisher feature direction 114 116  -->
![](https://web-api.textin.com/ocr_image/external/fc92c29745c88e6d.jpg)

Figure 3. Scatter plot in high-dimensional feature space.

dataset, which is generated from simulation studies, in the FCCU process and extracted from the first and second optimal discriminant vector using Fisher discriminant analysis. Then the data was projected to the optimal discriminant vector,which resulted in the generation of a scatter plot of the first and second feature vector in the original space. It can be seen in Fig. 2 that only fault 1 can be differentiated clearly from the normal data and that faults 2 and 3 cannot be differentiated from normal data. The reason for this is that FDA is a linear method in operation. Consequently, it has a poor ability to deal with data which shows complex nonlinear relationship among variables. The scatter plot of the frst kernel Fisher fea-ture vector and the second vector via kernel FDA is presented in Fig. 3. It is seen from Fig. 3 that after projecting to the high-dimensional feature space through selecting the appro-priate kernel function, the kernel Fisher discriminant method can easily discrimiate data that belong to different classes.

The RBF function is used as the selected kernel function, and the parameter c is selected as 0.8 according to experience, viz:

$K(x_{i},x_{j})=\exp (-\frac {\vert \vert x_{i}-x_{j}\vert \vert ^{2}}{c})$ (22)

The process disturbances considered are listed in Tab. 2.A 10% loss of combustion air blower capacity was selected for

Table 2.Process disturbances for FCCU.


| Case  | Disturbance  |
| -- | -- |
| 1  | 10% loss of combustion air blower capacity  |
| 2  | 5% degradation in the flow of regenerated catalyst  |
| 3  | 5% increase in the coke factor of the feed  |
| 4  | 10% decrease in the heat exchanger coefficient of the furnace  |
| 5  | 10% increase in fresh feed  |
| 6  | 5% decrease in lift air blower speed  |
| 7  | 5% increase in friction coefficient of regenerated catalyst  |
| 8  | Negative bias of reactor pressure sensor  |


