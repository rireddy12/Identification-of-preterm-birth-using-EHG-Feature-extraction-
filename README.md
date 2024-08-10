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

# Wavelet Decomposition
* Wavelet decomposition is done to know the frequency components in a non-stationary signal. Wavelet decomposition gives the time-frequency resolution.
* This helps us understand the frequency of electrical activity at a specific moment. 
* Biorthogonal wavelets are specifically chosen because they simplify reconstruction and do not introduce phase distortion.
* Signal decomposition is done in two different levels

# Sample Entropy
* Sample entropy is a metric used to quantify the complexity or regularity of a data series. It measures the likelihood that patterns in a time series that are similar will remain similar in the subsequent data points.
* It works by comparing patterns of length m within the time series to each other. These patterns are compared with a tolerance or similarity threshold r. Patterns are considered similar if their absolute difference is less than r.
* For each pattern of length m, sample entropy counts the number of similar patterns in the time series, then calculates the logarithm of the conditional probability that a pattern of length m+1 is similar, given that a pattern of length 𝑚 is similar. This is then averaged over all patterns.
* Lower values indicate the signal is regular and predictable whereas higher value indicates complexity and randomness. 

# Fractal Dimension
* Fractal dimension is a metric used to quantify the complexity of fractal objects. It measures how the detail in a fractal pattern changes with the scale at which it is measured.
* It works by analyzing how the number of self-similar pieces in the fractal changes with the scale. For a given fractal, the fractal dimension can be calculated using methods like box-counting, where the fractal is covered with a grid of boxes of size ε, and the number of boxes N(ε) that contain part of the fractal is counted. This process is repeated for different box sizes.
* For each box size ε, the number of boxes N(ε) that cover the fractal is determined, then the logarithm of N(ε) is plotted against the logarithm of 1/ε. The slope of the resulting line gives an estimate of the fractal dimension, D. This is often expressed as:
D=limϵ→0 ​log(1/ϵ)log(N(ϵ))​
* Lower values of fractal dimension indicate simpler, more regular structures, while higher values indicate more complex, intricate patterns. Fractal dimension is not necessarily an integer, reflecting the complex, often self-similar nature of fractal geometries.

# Conclusion
1. Wavelet decomposition with biorthogonal wavelets offers improved time-frequency resolution, aiding in understanding the frequency components of non-stationary signals without phase distortion.
2. Signal decomposition at two levels enhances spectral analysis, with higher spectral centroid values indicating frequency concentration at higher spectrum parts, and preterm signals displaying higher spectral flatness values, suggesting a more uniform spectrum.
3. Analysis of roll-off frequencies reveals differences in energy concentration among classes, with preterm signals having lower energy in higher frequencies compared to term and normal signals.
4. Features like sample entropy and fractal dimensions highlight complexity and randomness in EHG signals, with preterm signals showing higher complexity and variability in fractal dimension values compared to term and normal signals.
5. Overall, these techniques enable partial detection of preterm births by uncovering underlying patterns and complexities in EHG signals associated with preterm labor.





