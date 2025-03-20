```markdown
Chem. Eng. Technol. 2007, 30, No. 9, 1203-1211

## Table 1. Considered process variables of the FCCU case study.

| Variable | Description |
|----------|--------------|
| 1        | Flow of wash oil to reactor riser |
| 2        | Flow of fresh feed to reactor riser |
| 3        | Flow of slurry to reactor riser |
| 4        | Temperature of fresh feed entering furnace |
| 5        | Fresh feed temperature to riser |
| 6        | Furnace firebox temperature |
| 7        | Combustion air blower inlet suction flow |
| 8        | Combustion air blower throughput |
| 9        | Combustion air flow rate |
| 10       | Lift air blower suction flow |
| 11       | Lift air blower speed |
| 12       | Lift air blower throughput |
| 13       | Riser temperature |
| 14       | Wet gas compressor suction pressure |
| 15       | Wet gas compressor inlet suction flow |
| 16       | Wet gas flow to vapor recovery unit |
| 17       | Regenerator bed temperature |
| 18       | Stack gas valve position |
| 19       | Regenerator pressure |
| 20       | Standpipe catalyst level |
| 21       | Stack gas O2 concentration |
| 22       | Combustion air blower discharge pressure |
| 23       | Wet gas composition suction valve position |

## Figure 3. Scatter plot in high-dimensional feature space.

The process disturbances considered are listed in Tab. 2. A 10% loss of combustion air blower capacity was selected for Case 1. It is generated from the simulation and extracted in the FCCU process, which is generated from the simulation and extracted in the FCCU process, which is generated from the simulation. The data was projected to the optimal discriminant vector, which was obtained by applying Fisher discriminant analysis. Then the data was projected to the optimal discriminant vector, which was obtained by applying Fisher discriminant analysis.

The scatter plot of the first kernel Fisher feature vector is seen in Fig. 3. It is seen that after projecting the data to the first and second feature vector in the original space, it can be seen in Fig. 2 that only fault 1 can be differentiated clearly from the normal data and fault 2 and 3 cannot be differentiated clearly from normal data. The reason for this is that FDA is a linear method with operation. Consequently, it has a poor ability to deal with which complex nonlinear relationship among variables. The scatter plot of the first kernel Fisher feature vector is seen in Fig. 3. It is the second vector via kernel FDA is presented in the figure. It is seen that after projecting the data to the first and second feature vector in the original high-dimensional feature space through selecting the appropriate kernel function, the kernel Fisher discriminant method can easily discriminate the data belonging to different classes.

The RBF function is used as the selected kernel function, and the parameter c is selected as 0.8 according to experience, viz:

\[ K(x_i, x_j) = \exp \left( -\frac{\| x_i - x_j \|^2}{c} \right) \]

## Table 2. Process disturbances for FCCU.

| Case | Disturbance |
|------|---------------|
| 1    | 10% loss of combustion air blower capacity |
| 2    | 5% degradation in the flow of regenerated catalyst |
| 3    | 5% increase in the coke factor of the feed |
| 4    | 10% decrease in the heat exchanger coefficient of the furnace |
| 5    | 10% increase in fresh feed |
| 6    | 5% decrease in lift air blower speed |
| 7    | 5% increase in friction coefficient of regenerated catalyst |
| 8    | Negative bias of reactor pressure sensor |

## Figure 2. Scatter plot in original feature space.

© 2007 WILEY-VCH Verlag GmbH & Co. KGaA, Weinheim

http://www.cet-journal.com
```