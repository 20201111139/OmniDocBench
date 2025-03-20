```markdown
|Method|Data set|Subject|FI Score|Modality|Training Accuracy|Validation Accuracy|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|SVM EBF [18]|CASIA|75|0.890|RGB|0.90|0.89|
|Spoof ResNet [19]|MSU-MFSD|35|0.878|RGB|0.973|0.944|
|MTCNN [20]|YOUTU|3350|0.956|RGB/IR|0.962|0.978|
|SqueezeNet [21]|CASIA-SURF|1000|N/A|Color, Depth & IR|N/A|0.998|
|FusionNet|CASIA-SURF|300|0.998|Color, Depth & IR|0.997|0.998|

### 4. Conclusion

In this research, we used a deep learning method focused on Fusion CNN architecture to derive facial patches and depth of 3 types of human facial images. Color, Depth and IR from the CASIA-SURF dataset modeled with an altered 3D convolutional neural network classifier. Our primary interest was to be able to extract facial patches with a real face from a spoofed face from a CASIA-SURF dataset provided which are not preprocessed.

### Acknowledgements

This work is supported by Department of Science and Technology of Sichuan Province, China, under Grant 2019YJ0166.

### References

[1] J. Berry and D.A. Stoney. The history and development of fingerprinting. Advances in fingerprint technology, 2nd ed., 2001, 13-52.

[2] W. Yang, S. Wang, J. Hu, et al. Security and accuracy of fingerprint-based biometrics: A review. Symmetry, 2019, 11(2): 1-21.

[3] L. Intraona and H. Nissenbaum. Facial recognition technology: A survey of policy and implementation issues. J. Law, Info. & Sci., 2017, 1-38.

[4] D. Wen, H. Han, and A.K. Jain. Face spoof detection with image distortion analysis. IEEE Transactions on Information Forensics and Security, 2015, 10(4): 746-761.

[5] K.A. Nixon, V. Aimale, and R.K. Rowe. Handbook of biometrics. Springer, 2008, 403-423.

[6] A. da Silva Pinto, H. Pedrini, W. Schwartz, et al. Video-based face spoofing detection using convolutional neural networks. Graphics, Patterns and Images, 2012, 22(1): 221-228.

[7] A. Krizhevsky, I. Sutskever, and G.E. Hinton. Imagenet classification with deep convolutional neural networks. Advances in neural information processing systems, 2012, 421-436.

[8] Y. Atoum, Y. Liu, A. Jourabloo, et al. Face anti-spoofing using patch and depth-based CNNs. IEEE International Joint Conference on Biometrics (IJCB), 2017, 1-8.

[9] J. Qiu, J. Cai, M. Tian, et al. Biometrics (IJCB), 2017, 1-8.

[10] S. Lawrence, C.L. Giles, A.C. Tsoi, et al. Face recognition: A convolutional neural-network approach. IEEE Transactions on Neural Networks, 1997, 8(1): 98-113.

[11] Z. Zhang, J. Yan, S. Li, et al. A face antispoofing database with software-based 2D attack detection. IEEE International Conference on Biometrics (ICB), 2012, 26-31.

[12] A. Alkari and S. Alghowinem. The effectiveness of depth data in liveness face authentication using 3D sensor cameras. IEEE Sensors Journal, 2019, 19(8): 1928-1937.

[13] J. Sensors, J. Sensors, 2018, 1-8.

[14] C.-L. Zhang, J.-H. Liao, X.-S. Wei, et al. In defense of fully convolutional networks for transfer learning. IEEE Transactions on Image Processing, 2018, 27(1): 1-12.

[15] J. Konečný, J. Liu, P. Richtárik, et al. Mini-batch semi-stochastic gradient descent in the proximal setting. IEEE Journal of Selected Topics in Signal Processing, 2015, 9(4): 242-255.

[16] A.F. Agarap. Deep learning using rectified linear units (ReLU). arXiv preprint arXiv:1803.08375, 2018.

[17] L. Bottou. Neural networks: Tricks of the trade. Springer, 2012, 421-436.

[18] M. Hardt, B. Recht, and Y. Singer. Train faster, generalize better: Stability of stochastic gradient descent. arXiv preprint arXiv:1509.01240, 2015.

[19] D.T. van der Haar. Face Antispoofing Using Shearlets: An Empirical Study. Journal of SAI, 2019, 110(2): 94-103.

[20] C. Nagpal and S.R. Dubey. A performance evaluation of convolutional neural networks for face and anti spoofing. IEEE Transactions on Information Forensics and Security, 2018, 13(10): 2496-2509.

```