# 283

Fig: Test images superimposed: in red the first, in green the second frame (left). The white square indicates the Interrogation Window. On the right the same image with rectangular artificially saturated area on the first frame.

|15|Lorentzian|15|SSD|15|Fast Correlation|
|---|---|---|---|---|---|
|10| |10| |-10| |
|15|10|10|-15|-10|10|

Fig: 3 Maps of dissimilarity with Lorentzian sum of squared 0.7, 0.6 and 0.5 are drawn in red, green, and blue, respectively. The dissimilarity are subtracted of the lowest minimum value and normalized by the maximum value. Contours are drawn from 0 to with a step of 0.05. For reference, the levels represent guessed displacement in the x and y direction respectively.

Fig: Dissimilarity maps on the modified image. Same contour lines and axes as in Fig.

|15|Lorentzian| |SSD| |Fast Correlation|
|---|---|---|---|---|---|
|10| |10| |10| |
|10| |10| |10| |
|-15|-10|10|-15|-10|10|

Conservation by spurious pixels (outliers) between (e.g- the white square artificially added in the first frame). The SSD and cross-correlation are functions defined univocally. Conversely, the Lorentzian depends on parameter, Ge, which tunes how robust the estimator has to be. As a matter of fact, it should equal the amplitude of the expected differences between pixels fulfilling the BCC. The above maps have been computed with a value equal to 26, that is about one half of the standard deviation of the image gray levels (o 43 1 0.1 for both images).

In order to test the sensitivity of the solution on the parameter Ge; the dissimilarity map given by the Lorentzian estimator was computed for six different values of Ge, ranging from 2 to 128; results are plotted in Fig 5. If one assumes the level of the second peak as an indication of the signal to noise ratio, one should conclude that the values of 26 is not optimal, since the values from 3 up to 13 behaves slightly better; but the results are more or less similar to those obtained with 26. Further increases of the value deteriorate the S/N ratio but also for 6e 128, the Lorentzian estimator works noticeably better than SSD or cross-correlation. These results indicate that the Lorentzian estimator performs well for wide range of values of the parameter, even though the optimal seems to be at about 1/3 of the.