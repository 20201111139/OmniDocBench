# Chem: Eng: Technol. 2007 , 30, No. 9, 1203-1211

# Real-time processes

# Table 1. Considered process variables of the FCCU case study:

|Variable|Description|normal|fault1|fault2|fault3| | | |
|---|---|---|---|---|---|---|---|---|
| |Flow of wash oil to reactor riser|1| | | | | | |
| |Flow of fresh feed to reactor riser|1|3.6| | | | | |
|Flow of slurry to reactor riser| | | | | | | | |
| |Temperature of fresh feed entering furnace|2| | | | | | |
| |Fresh feed temperature to riser|1| | | | | | |
| |Furnace firebox temperature|3|2.8| | | | | |
| |Combustion air blower inlet suction flow| | | | | | | |
| |Combustion air blower throughput|2.6| | | | | | |
| |Combustion air flow rate|404|106|108|110|112|114|116|
| |Lift air blower suction flow|10| | | | | | |
|Lift air blower speed|11| | | | | | | |
| |Lift air blower throughput|12| | | | | | |
| |Riser temperature|13| | | | | | |
| |Wet gas compressor suction pressure|14| | | | | | |
| |Wet gas compressor inlet suction flow|15| | | | | | |
| |Wet gas flow to vapor recovery unit|16| | | | | | |
| |Regenerator bed temperature|17| | | | | | |
| |Stack gas valve position|18| | | | | | |
| |Regenerator pressure|19| | | | | | |
| |Standpipe catalyst level|20| | | | | | |
|Stack gas O2 concentration|21| | | | | | | |
|Combustion air blower discharge pressure|22| | | | | | | |
|Composition suction valve position|23| | | | | | | |

Figure 3. Scatter plot in high-dimensional feature space dataset; which is generated from simulation studies, in the FCCU process and extracted from the first and second optimal discriminant vector using Fisher discriminant analysis. Then the data was projected to the optimal discriminant vector; which resulted in the generation of a scatter plot of the first and second feature vector in the original space. It can be seen in Fig: 2 that only fault 1 can be differentiated clearly from the normal data and that faults 2 and 3 cannot be differentiated from normal data. The reason for this is that FDA is a linear method in operation. Consequently, it has poor ability to deal with data which shows complex nonlinear relationships among variables. The scatter plot of the first kernel Fisher feature vector and the second vector via kernel FDA is presented in Fig: 3. It is seen from Fig: 3 that after projecting to the high-dimensional feature space through selecting the appropriate kernel function, the kernel Fisher discriminant method can easily discriminate data that belong to different classes. The RBF function is used as the selected kernel function, and the parameter c is selected as 0.8 according to experience, viz: K(xi,;) = exp(-h 4l).

# Table 2. Process disturbances for FCCU

|Case|Disturbance|
|---|---|
|1|10 % loss of combustion air blower capacity|
|2|5 % degradation in the flow of regenerated catalyst|
|3|5 % increase in the coke factor of the feed|
|4|10 % decrease in the heat exchanger coefficient of the furnace|
|5|10 % increase in fresh feed|
|6|5 % decrease in lift air blower speed|
|7|5 % increase in friction coefficient of regenerated catalyst|
|8|Negative bias of reactor pressure sensor|

2007 WILEY-VCH Verlag GmbH & Co. KGaA, Weinheim

http://www.cet-journal.com