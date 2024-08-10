# Identification-of-preterm-birth-using-EHG-Feature-extraction-
Estimation of preterm birth before 34 weeks of pregnancy

# Introduction
Preterm birth is defined as birth before 37 weeks of pregnancy. The World Health Organization has reported that every year about 15 million newborns are preterm, which accounts for more than 10% of all babies born around the world. Preterm birth is a dominant cause of morbidity and mortality during both the perinatal and early neonatal periods. In addition, the complications of preterm birth such as significant neurological, mental, behavioral, and pulmonary problems have a significant adverse impact on family and the economy.

# Objective
1. Develop a robust feature extraction pipeline from EHG signals to detect preterm birth, focusing on extracting relevant features from the signal's spectrogram, including sample entropy, and fractal dimensions.
2. Implement preprocessing techniques such as Butterworth filtering (0.5-4Hz) to enhance the signal quality and remove noise, ensuring the accuracy of subsequent analysis steps.
3. Utilize wavelet decomposition with biorthogonal wavelets to effectively capture both time and frequency domain features of the EHG signal, facilitating comprehensive feature extraction.
4. Leveraging the extracted features to accurately identify preterm births, particularly focusing on predicting births occurring before the 37th week of pregnancy.
5. Address the significant medical and economic challenges posed by preterm birth by providing effective methods for its detection or prediction, aiming to reduce its incidence and improve outcomes for both infants and families.

# Flowchart

# Conclusion
1. Wavelet decomposition with biorthogonal wavelets offers improved time-frequency resolution, aiding in understanding the frequency components of non-stationary signals without phase distortion.
2. Signal decomposition at two levels enhances spectral analysis, with higher spectral centroid values indicating frequency concentration at higher spectrum parts, and preterm signals displaying higher spectral flatness values, suggesting a more uniform spectrum.
3. Analysis of roll-off frequencies reveals differences in energy concentration among classes, with preterm signals having lower energy in higher frequencies compared to term and normal signals.
4. Features like sample entropy and fractal dimensions highlight complexity and randomness in EHG signals, with preterm signals showing higher complexity and variability in fractal dimension values compared to term and normal signals.
5. Overall, these techniques enable partial detection of preterm births by uncovering underlying patterns and complexities in EHG signals associated with preterm labor.





