Fig.2 Test images superimposed: in red the first,in green the second frame (left).The white square indicates the Interrogation Window. On the right the same image with a rectangular artificially saturated area on the first frame


![](https://web-api.textin.com/ocr_image/external/3ea3c1cb8029b1a0.jpg)


![](https://web-api.textin.com/ocr_image/external/04d9a5203fbb9a51.jpg)

<!-- 15 Lorentzian 10 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/6459f7a2345098cc.jpg)

<!-- 15 SSD 10 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/6689211d47f02dd2.jpg)

<!-- 15 Fast Correlation 10 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/51401d5d5fab8312.jpg)

Fig.3 Maps of dissimilarity with Lorentzian, sum of squared differences and fast correlation.Dissimilarity are subtracted of the minimum value and normalized by the maximum value. Contours are drawn from 0 to 1 with a step of 0.05.For reference,the levels

0.7,0.6 and 0.5 are drawn in red, green, and blue, respectively.The lowest the dissimilarity the darker the background. Abscissa and ordinate represent guessed displacement in the x and y direction,respectively

Fig.4 Dissimilarity maps on the modified image.Same contour lines and axes as in Fig. 3

<!-- 15 Lorentzian 10 4 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/c48bbaf11c03f7e1.jpg)

<!-- 15 SSD 10 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/9f6ffaab01260ba5.jpg)

<!-- 15 Fast Correlation 10 5 0 -5 -10 -15 -10 0 10  -->
![](https://web-api.textin.com/ocr_image/external/a140efb476e2a9d2.jpg)

conservation by spurious pixels (outliers) between (e.g.the white square artificially added in the first frame).

The SSD and cross-correlation are functions defined univocally.Conversely, the Lorentzian depends on a parameter,$\sigma _{e}$which tunes how robust the estimator has to be. As a matter of fact, it should equal the amplitude of the expected differences between pixels fulfilling the BCC.The above maps have been computed with a value equal to 26, that is about one half of the standard deviation of the image gray levels(σ=43±0.1 for both images).

In order to test the sensitivity of the solution on the parameter oe,the dissimilarity map given by the

Lorentzian estimator was computed for six different values of$\sigma _{e},$ranging from 2 to 128; results are plotted in Fig. 5. If one assumes the level of the second peak as an indication of the signal to noise ratio, one should con-clude that the values of 26 is not optimal,since the values from 3 up to 13 behaves slightly better, but the results are more or less similar to those obtained with 26.Further increases of the value deterioratetheS/Nratio,but also for$\sigma _{}=128,$the Lorentzian estimator works noticeably better than SSD or cross-correlation. These results indicate that the Lorentzian estimator performs well for a wide range of values of the parameter, even though the optimal seems to be at about 1/3 of the

