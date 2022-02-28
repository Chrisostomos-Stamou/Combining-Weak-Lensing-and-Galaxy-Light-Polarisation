# Combining-Weak-Lesning-and-Galaxy-Light-Polarisation
This repository contains my MSc Thesis, titled "Combining Weak Lensing and Galaxy Light Polarisation" and the Python codes I used to derive some plots and results for my research.   

Specifically, this Thesis investigates if polarisation can bring extra information to weak lensing measurements. This involves constructing an optimal estimator for shear that includes polarisation and then measuring shear correlation functions by using the usual estimator for shear-averaging observed ellipticity- and the optimal one. Comparing the variance between those two estimators, we can work out then noise that each estimator brings to the measurement. The correlation between polarisation and intrinsic ellipticity is characterised by two parameters: P and \sigma_{p}, where \sigma_{p} is the dispersion in the polarisation measurement and P defines the "strength" of the correlation. Thus, the optimal estimator is calculated for different values of P and we fix \sigma_{p} to be equal to 0.25.


In the file "Opt_Shear_cf.ipynb" we compute these correlation functions using simulated data sets (https://slics.roe.ac.uk/) and we find that the optimal estimator is less noisy than the usual one, provided that polarisation is correlated to the intrinsic ellipticity. For measuring shear correlation functions, we used TreeCorr (https://rmjarvis.github.io/TreeCorr/_build/html/index.html)


What is mentioned above is the most important part of the project. Besides that, we test the effect of polarisation into weak lensing measurements in the following thwo ways:
1) In the file "Optimal Estimator.ipynb" we generate random galaxy catalogues by generating random intrinsic ellipticities given by a normal distribution with dispersion se=0.25 and we assume a given shear. Given that, we can calculate the observed ellipticity and then the polarisation for each galaxy and eventually compare the variance of the optimal estimator for different values of P to the variance of the usual one. We find that the more correlated polarisation and intrinsic ellipticty are, the smaller the variance of the optimal estimator compared to that of the usual estimator. 
2) In the file "MOCK.ipynb", we use the KiDS-450 Mock Source catalogue which gives a catalogue of shear and observed ellipticity and we repeat the same process. We find again the same result.


The pdf file is the Thesis text, where guidelines regarding the codes are given.
