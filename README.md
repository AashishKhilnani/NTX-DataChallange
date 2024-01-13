# NTX-DataChallange

We have focused on feature extraction. We have used Empirical Wavelet Transform (EWT) to decompose the signals into 3 Intrinsic Mode Functions (IMF). These IMFs have better resolution of time domain features. Thus we extracted variance, skewness, kurtosis, Point to point range, Root mean square, Standard deviation, number of zero crossings, hjorth mobility and hjroth complexity, Petrosian fd and permutation entropy from each of the 3 IMFs. 

This gives us 11*3 = 33 features from the time-frequency domain per signal. 

Then we used the Welch method to extract the Power Spectral Density function across various bands, as well as the ratios of power across bands. 

This gives us a total of 9 frequency domain features per signal. 

Moreover, we also extracted the correlation between the two signals. Thus we have a total of  2(33+9)+1=85 features. 

The Python notebook is given in the repository. 

