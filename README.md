# speech_features-mfcc-dft

1)Divide input speech signal into frames with 50% overlap.

2)Take window size same as that of the size of frames and multiply it with the frames. In this case, hamming window is taken.

3)Take DFT  framewise. Equation for calculating discrete fourier transform is given by:

![Image of dft](https://github.com/GurudasKarale/speech_features-mfcc-dft-/blob/master/img/dft.PNG)

4)Sum up the energy of each frame

5)Take the logarithm of all energies.

6)Pass it through the mel filter bank. Transfer function of filter bank is giver by:

![Image of transfer](https://github.com/GurudasKarale/speech_features-mfcc-dft-/blob/master/img/tra.PNG)

7)Take the DCT of the log filterbank energies and keep 2-13 coefficients.

