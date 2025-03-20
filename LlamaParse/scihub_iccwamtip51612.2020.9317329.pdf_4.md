# Table 4 Comparison review with existing_work's methods and accuracy scores

|Method|Data set|Subject|F Score|Modality|Training accuracy|Validation Accuracy|
|---|---|---|---|---|---|---|
|SVM EBF [18]|CASIA|0.890|RGB|0.90|0.89| |
|Spoof ResNet [9]|MSU-MFSD|NIA|RGB|0.978|0.944| |
|MTCNN [20]|YOUTU|3350|0.956|RGB/IR|0.962|0.978|
|SqueezeNet [21]|CASIA-SURF|1000|N/A|Color; Depth & IR|N/A|0.998|
|FusionNet|CASIA-SURF|300|0.998|Color Depth & IR|0.997|0.998|

# Conclusion

In this research, we used deep learning methods focused on Fusion CNN architecture to derive facial patches and depth of 3 types of human facial image samples namely Color; Depth and IR from the CASIA-SURF dataset modeled with an altered 3D convolutional neural network classifier. Our primary interest was to be able to extract facial patches and the depth levels of all 3 facial inputs stated earlier on to distinguish a real face from a spoofed face from a CASIA-SURF dataset provided which are not preprocessed.

# Acknowledgements

This work is supported by the Department of Science and Technology of Sichuan Province, China, under Grant 2019YJO166.

# References

1. Berry and D.A. Stoney: The history and development of fingerprinting [J]: Advances in fingerprint technology 2001, 2.13-52
2. W. Yang; Wang: Hu, et al. Security and accuracy of fingerprint-based biometrics: review [J]: Symmetry; 2019, 1(2):141.
3. Introna and Nissenbaum Facial recognition technology survey of policy and implementation [J]: 2010.
4. D. Wen, H. Han, and A. K Jain. Face detection spoof with image distortion analysis [J]: IEEE Transactions on Information Forensics and Security, 2015, 10(4):746-761.
5. KA Nixon, V Aimale, and R K Rowe Handbook of biometrics. 2008.403-423
6. A. da Silva Pinto. H. Pedrini. W. Schwartz et al. Video-based face spoofing detection through visual rhythm analysis [C].2012 25th SIBGRAPI Conference on Graphics Patterns and Images, 2012, 221-228.
7. Krizhevsky; Sutskever; and Hinton. Imagenet classification with deep convolutional neural networks [C]: Advances in neural information processing systems; 2016, 379-387.
8. M: Hardt; Recht; and Y Singer: Train faster; generalize better: Stability of stochastic gradient descent [J]: arXiv preprint arXiv:1509.01240, 2015
9. D. van der Haar: Face Antispoofing Using Shearlets: An Empirical Study [J]: SAIEE Africa Research Journal, 2019, 110(2):94-103.
10. Nagpal and S R Dubey: A performance evaluation of convolutional neural networks for face anti spoofing.