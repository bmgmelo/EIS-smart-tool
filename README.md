# EIS-analysIS
EIS analysIS is a standalone MATLAB application software for the visualization, analysis, and modeling of impedance spectroscopy data.

**To run the software, download the EIS_analysIS_for_testing rar file.**

You can use the "YSZ_table_example.txt" file to test the software. This file includes some impedance measurements of a YSZ pellet, as a function of temperature (temperature values in Kelvin) and frequency. Load this file with "Load existing file" option. An instructional video of how to use the software will be added in a short time.

The user can load a text file with the Z’ and -Z’’ values of each frequency and temperature (example in next Table) and the software will calculate all the remaining immittance functions. The resulting matrix can be saved and conveniently reloaded every time the user wishes to perform further analysis.

![imagem](https://user-images.githubusercontent.com/42448042/205509349-ee4ed2b2-4ddb-4189-a6ae-ef180a71904d.png)

The application software allows to import and analyze isolated EIS data measured at a single temperature, however, it is especially useful for the analysis of impedance data as a function of temperature. All graphics are customizable with multiple line styles, maker styles, colormaps, and the user can choose to save them as an image file or export the selected data as a text file.

The application software provides the ability to study the dielectric relaxations according to different models. Some of the most relevant features are:

▪ Fitting the impedance data (real and imaginary parts of impedance) to a user-defined equivalent circuit model;

▪ Evaluating the fit residuals, export (as text or image) the complex impedance fit and the fitted parameters;

▪ Fitting complex data (Impedance, Dielectric Modulus, and Permittivity) according to the Havriliak-Negami function. The fitting is performed to both real and imaginary parts of the complex function;

▪ Calculating the Havriliak-Negami fit residuals and exporting the fitted curves as a text file or a customizable image;

▪ Studying the impedance data with the distribution function of relaxation times formalism (impedance data is directly imported to the DRTtools [1]);

▪ Checking the validity of the calculated distribution function of relaxation times, by the transforming the data into a synthetic impedance spectrum that can be compared with the original measured impedance data (DFRTtoEIS);

▪ Calculating the individual parameters including resistance, capacitance and time constants from the distribution function of relaxation times analysis (DFRTtoEIS);

▪ Exporting the impedance data in the adequate data type to check the internal consistency of the measured impedance with the Kramers-Kronig test (using an additional MATLAB tool – LIN KK [2]);

▪ Calculating the Nyquist plots in several immittance functions (Impedance, Dielectric Modulus, and Permittivity);


Further discussion can be found in: "DFRTtoEIS: An easy approach to verify the consistency of a DFRT generated from an impedance spectrum" https://doi.org/10.1016/j.electacta.2020.137429


[1] T.H. Wan, M. Saccoccio, C. Chen, F. Ciucci, Influence of the Discretization Methods on the Distribution of Relaxation Times Deconvolution: Implementing Radial Basis Functions with DRTtools, Electrochim. Acta. 184 (2015) 483–499. https://doi.org/10.1016/j.electacta.2015.09.097.

[2] M. Schönleber, D. Klotz, E. Ivers-Tiffée, A Method for Improving the Robustness of linear Kramers-Kronig Validity Tests, Electrochim. Acta. 131 (2014) 20–27. https://doi.org/10.1016/j.electacta.2014.01.034.
