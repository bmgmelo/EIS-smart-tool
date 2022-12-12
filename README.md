# EIS smart tool (Windows version)
EIS smart tool is a standalone MATLAB application software for the visualization, analysis, and modeling of impedance spectroscopy data.

**How to install the software:**

**1) Download and install the Windows version of the MATLAB Runtime for R2017b from the following link on the MathWorks website: http://www.mathworks.com/products/compiler/mcr/index.html**

**2) Download the EIS-smart-tool rar file**

**3) Extract files from the rar** 

**4) Run the EIS smart tool.exe** 

You can use the "YSZ_table_example.txt" file (available in the rar file) to test the software. This file includes some impedance measurements of a YSZ pellet, as a function of temperature (temperature values in Kelvin) and frequency. **Load this file with "Load existing file" option and press run**. 

**Please check the instructional videos of how to use the software.**

**Starting guide video: https://youtu.be/Hxky_bsu2Kw**

**Load new data video: https://youtu.be/KChpUhqamAE**

**EIS smart tool Havriliak–Negami (HN) example 1: https://youtu.be/7BxeiYYCRTE**

**EIS smart tool Havriliak–Negami (HN) example 2: https://youtu.be/Qva4HT9Yg1A**

**Other how to videos available https://www.youtube.com/@eis-smart-tool**



The user can load a text file with the Z’ and -Z’’ values of each frequency and temperature (example in next Table) and the software will calculate all the remaining immittance functions. The resulting matrix can be saved and conveniently reloaded every time the user wishes to perform further analysis.

![imagem](https://user-images.githubusercontent.com/42448042/205509349-ee4ed2b2-4ddb-4189-a6ae-ef180a71904d.png)

The application software allows to import and analyze isolated EIS data measured at a single temperature, however, it is especially useful for the analysis of impedance data as a function of temperature. All graphics are customizable with multiple line styles, maker styles, colormaps, and the user can choose to save them as an image file or export the selected data as a text file.

The application software provides the ability to study the dielectric relaxations according to different models. Some of the most relevant features are:

▪ Fitting the impedance data (real and imaginary parts of impedance) to some predefined equivalent circuit models, or a user-defined circuit (for the latter option the program uses the Zfit tool available in [1];

▪ Evaluating the fit residuals, export (as text or image) the complex impedance fit and the fitted parameters;

▪ Fitting complex data (Impedance, Dielectric Modulus, and Permittivity) according to the Havriliak-Negami function. The fitting is performed to both real and imaginary parts of the complex function;

▪ Calculating the Havriliak-Negami fit residuals and exporting the fitted curves as a text file or a customizable image;

▪ Studying the impedance data with the distribution function of relaxation times formalism (impedance data is directly imported to the DRTtools [2]);

▪ Checking the validity of the calculated distribution function of relaxation times, by the transforming the data into a synthetic impedance spectrum that can be compared with the original measured impedance data (DFRTtoEIS);

▪ Calculating the individual parameters including resistance, capacitance and time constants from the distribution function of relaxation times analysis (DFRTtoEIS);

▪ Exporting the impedance data in the adequate data type to check the internal consistency of the measured impedance with the Kramers-Kronig test (using an additional MATLAB tool – LIN KK [3]);

▪ Calculating the Nyquist plots in several immittance functions (Impedance, Dielectric Modulus, and Permittivity);

▪ Calculating the Arrhenius representation and determining the activation energy of the electrical conductivity (σ’) over the desired temperature range;

▪ Fitting the ac conductivity (σ’) data using Jonscher’s power law;

▪ Providing analysis tools for distinguishing between the long-range conductivity peak and the localized relaxation processes;

▪ Evaluating the scaling behavior of a dielectric relaxation with the master curve;

▪ Applying the derivative method (εder′′).

If you found this work helpful, please consider citing the following article: "DFRTtoEIS: An easy approach to verify the consistency of a DFRT generated from an impedance spectrum" https://doi.org/10.1016/j.electacta.2020.137429


Please let me know if you find some bugs while using the software. Further updates will be added in the future.
Bruno Melo (bmelo@ua.pt)
________________________________________________________________________________________________________________________________________________________
References

[1] J.-L. Dellis, Zfit, (n.d.). https://www.mathworks.com/matlabcentral/fileexchange/19460-zfit.

[2] T.H. Wan, M. Saccoccio, C. Chen, F. Ciucci, Influence of the Discretization Methods on the Distribution of Relaxation Times Deconvolution: Implementing Radial Basis Functions with DRTtools, Electrochim. Acta. 184 (2015) 483–499. https://doi.org/10.1016/j.electacta.2015.09.097.

[3] M. Schönleber, D. Klotz, E. Ivers-Tiffée, A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests, Electrochim. Acta. 131 (2014) 20–27. https://doi.org/10.1016/j.electacta.2014.01.034.
