## 4 Conclusion

we used a focused on Fusion CNN architecture to derive facial patches and depth of 3 types of human facial image samples namely Color; Depth and IR from the CASIA-SURF dataset modeled with an altered 3D convolutional neural network classifier. Our primary interest was to be able to extract facial patches and the depth levels of all 3 facial inputs stated earlier on to distinguish a real face from a spoofed face from CASIA SURF dataset provided which are not preprocessed.

## Acknowledgements

Technology of Sichuan   Province, China, under Grant 2019YJ0166.

## References

- [1] J of fingerprinting [J] Advances in fingerprint Technology; 2001,2:13-52. Berry
- of fingerprint-based biometrics: A review [J] Symmetry; 2019, 11(2):141 .
- [4] D. K. Jain. Face detection with image distortion analysis [J]. IEEE Transactions on Information Forensics and Securitys 2015, 10(4).746-761. spoof
- [3] L. Introna and Facial   recognition technology a survey and   implementation issues [J].2010.
- [5] biometrics; 2008, 403-423.
- [6] based face spoofing detection through visual rhythm 25th SIBGRAPI Conference on Graphics; Patterns and Images, 2012, 221-228.

methods and accuracy scores

| Method            | Data set   | Subject   | Fl Score   | Modality          | Training Accuracy   |   Validation Accuracy |
|-------------------|------------|-----------|------------|-------------------|---------------------|-----------------------|
| SVM EBF [18]      | CASIA      | 75        | 0.890      | RGB               | 0.90                |                 0.89  |
| Spoof ResNet [19] | MSU-MFSD   | 35        | NA         | RGB               |                     |                 0.944 |
| MTCNN [20]        | YOUTU      | 3350      | 0.956      | RGB/IR            | 0.962               |                 0.978 |
| SqueezeNet [21]   | CASIA-SURF | 1000      | NIA        | Color; Depth & IR |                     |                 0.998 |
| FusionNet         | CASIA-SURF |           | 0.998      | Color; Depth & IR | 0.997               |                 0.998 |

- networks [C] Advances in neural information
- [8] spoofing and depth-based CNNs [C].2017 IEEE International Joint Conference Biometrics (IJCB), 2017,319328. using patch
- [9] identification from a depth camera [C] Proceedings of the International Conference on Pattern
- [10] S Lawrence, C. L Giles, A C. Tsoi, et al. Face recognition: A convolutional neural-network approach IEEE transactions neural networks, 1997 8(1).98-113 .
- Yan, al. A face   antispoofing database with diverse attacks [C].2012 5th IAPR international   conference on Biometrics (ICB), 2012,
- Alghowinem:  The effectiveness of depth   data in liveness 3D sensor cameras using
- [13] J region-based fully convolutional networks [C] Advances in neural information   processing systems; 2016, 379-387.
- fully connected layers in visual representation transfer [C] Pacific Rim Conference on Multimedia; 2017, 807-817.
- stochastic gradient descent in the proximal setting [J] IEEE Journal of Selected Topics in Signal Processing,
- [16] A F. Agarap. Deep learning rectified linear units using
- [17] L 421-436.
- Hardt, B Recht, and Y Train   faster; generalize better: Stability of stochastic   gradient Singer.
- [19] D. T. van der Haar: Face Antispoofing Shearlets: An Empirical Study [J] SAIEE Africa Research Journal, 2019,110(2).94-103 . Using
- [7] A Krizhevsky; Sutskever; and G. E Hinton. Imagenet classification with convolutional neural deep

- R Dubey. A performance evaluation of convolutional neural networks for face anti spoofing