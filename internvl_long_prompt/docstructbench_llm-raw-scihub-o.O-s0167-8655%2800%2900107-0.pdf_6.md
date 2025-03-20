```markdown
254

A. Sibert / Pattern Recognition Letters 22 (2001) 249-256

Fig. 5. Mag-Lap 2-D feature histograms for invariant representation of image ToolA: (a) OGC, 8 × 8; (b) CGC, 8 × 8; (c) OGC, 32 × 32; (d) CGC, 32 × 32. The gradient magnitude is along the vertical axis, the Laplacian along the horizontal axis.

Table 1

Distance matrix for intensity images, χ² metric, 8 × 8 bins, σpre = 0°

|          | Build | WoBA | WoBB | WoBC | WoBD | Cycl | Sand | ToolA | ToolB | ToolC |
|----------|-------|------|------|------|------|------|------|--------|--------|--------|
| Build     | 204.7 | 95.9 | 1915.3 | 1100.7 | 183.8 | 169.4 | 1889.2 | 1978.0 | 3546.3 | 2322.3 |
| WoBA      | 2018.0 | 490.3 | 169.2 | 982.4 | 128.4 | 2488.2 | 2458.4 | 466.6 | 124.3 | 592.0 |
| WoBB      | 4214.7 | 2011.2 | 603.5 | 993.4 | 1856.8 | 1825.9 | 1240.0 | 578.6 | 1167.5 | 1092.1 |
| WoBC      | 943.9 | 843.8 | 740.2 | 469.7 | 381.7 | 129.2 | 949.0 | 1040.3 | 154.1 | 1028.1 |
| WoBD      | 4081.1 | 3930.7 | 493.5 | 2246.0 | 1133.9 | 803.2 | 1182.5 | 2003.1 | 1443.4 | 2012.1 |
| Cycl       | 1455.0 | 1154.3 | 1927.1 | 1062.2 | 1039.5 | 1398.4 | 1237.9 | 1803.1 | 2694.5 | 2238.1 |
| Sand       | 1430.8 | 1394.8 | 1046.2 | 1321.5 | 1111.1 | 1240.1 | 2348.5 | 3201.0 | 2489.2 | 2134.1 |
| ToolA      | 3302.8 | 1326.8 | 1326.8 | 1326.8 | 1326.7 | 1326.7 | 1326.7 | 1326.7 |      |      |
| ToolB      | 1326.8 | 1326.8 | 1326.8 |      |      |      |      |      |      |      |
| ToolC      | 3540.1 | 1668.4 | 1079.5 | 1717.9 | 1233.2 | 2288.5 | 2503.6 | 380.5 | 261.8 | 310.4 |

*Minimum distances in bold face.

Table 2

Distance matrix for invariant representations, χ² metric, 8 × 8 bins, σpre = 1°

|          | Build | WoBA | WoBB | WoBC | WoBD | Cyl | Sand | ToolA | ToolB | ToolC |
|----------|-------|------|-------|------|------|------|------|--------|--------|--------|
| Build     |   136.1 |  353.1 |  523.7 |  352.9 |  134.8 |  647.1 |  1411.8 |  715.5 |  618.7 |  1215.1 |
| WoBA      |   613.5 |  579.0 |  236.6 |  249.4 |  347.8 |  168.3 |  482.3 |  144.0 |  141.7 |  395.9 |
| WoBB      |   517.4 |  307.0 |  260.0 |  343.4 |  240.1 |  640.7 |  768.5 |  140.7 |  174.4 |  340.4 |
| WoBC      |   484.3 |  263.3 |  234.5 |  85.2 |  656.9 |  362.7 |  787.3 |  286.1 |  254.7 |  517.8 |
| WoBD      |  1703.0 |  1661.0 |  610.6 |  740.2 |  579.1 |  315.8 |  404.0 |  168.2 |  463.5 |  259.6 |
| Cyl        |   753.3 |  565.0 |  670.5 |  312.3 |  579.7 |  315.9 |  193.6 |  368.2 |  465.3 |  309.0 |
| Sand       |  1834.4 |  587.9 |  999.8 |  920.4 |  402.7 |  268.5 |  60.9 |  59.1 |  71.6 |  69.1 |
| ToolA      |   833.8 |  833.8 |  833.8 |  833.8 |  220.2 |  220.2 |  220.2 |  220.2 |      |      |
| ToolB      |  1240.5 |  395.4 |  342.1 |  437.3 |  176.5 |  251.8 |  642.4 |  136.2 |      |      |
| ToolC      |  1240.5 |  342.1 |  342.1 |  437.3 |  176.5 |      |      |      |      |      |

*Minimum distances in bold face.

representation are more equally distributed over all histogram bins.

The χ² distances for the images in our test database, for 8 × 8 bins, are given in Table 1 for the intensity images without pre-filtering, and in Table 2 for the invariant representations with gentle Gaussian pre-filtering, σpre = 1.0. Each row shows the distances from the given OGC histograms to the CGC histograms. Note that the tables are not symmetric. If the χ² value is smallest on the diagonal, then the query image has been correctly recognized. The percentage of
```