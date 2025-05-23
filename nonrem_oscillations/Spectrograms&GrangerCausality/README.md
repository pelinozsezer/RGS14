# :sparkles: Spectrograms & Granger Causality :sparkles:
:pushpin: **Requirements**: [FieldTrip](https://github.com/fieldtrip/fieldtrip), [N-dimensional histogram](https://www.mathworks.com/matlabcentral/fileexchange/23897-n-dimensional-histogram), [Image Processing Toolbox](https://www.mathworks.com/products/image.html), [Statistics and Machine Learning Toolbox](https://www.mathworks.com/products/statistics.html), [Signal Processing Toolbox](https://www.mathworks.com/products/signal.html), [Deep Learning HDL Toolbox](https://www.mathworks.com/products/deep-learning-hdl.html), [Wavelet Toolbox](https://www.mathworks.com/products/wavelet.html), [Symbolic Math Toolbox](https://www.mathworks.com/products/symbolic.html), [Computer Vision Toolbox](https://www.mathworks.com/products/computer-vision.html), [Bioinformatics Toolbox](https://www.mathworks.com/products/bioinfo.html).


------------------------------------

<a href="url"><img src="https://github.com/pelinozsezer/RGS14/blob/main/nonrem_oscillations/Spectrograms%26GrangerCausality/pipeline.png" align="center" height="500" width="525" ></a>

------------------------------------

- **MAIN_script_ripples_pca_threshold_gmm.m**: Extracts ripples from waveforms; Generates the data of features; Normalizes and computes PCA; Generates density maps; Thresholds; Fits GMM model; Finds clusters per treatment; Creates new files per cluster and per treatment.

- **split_waveforms_all.m**: Finds visually inspected missing data and replaces them with the proper data; Sorts out the data per rat and per study day.

- **GC_ripple_4clusters_median_wa.m**: Prepares data for spectrograms and Granger analysis; Finds the 2000 ripples closest to the median in amplitude; Removes artifacts.

- **spectrogram_main.m**: Generates spectrograms and contrasts; Runs statistics on contrasts.

- **granger_main.m**: Generates Granger Analysis plots and contrasts; Runs statistics on contrasts.

------------------------------------

:exclamation: Section 2 of _GC_ripple_4clusters_median_wa.m_ should be run cluster by cluster. Threshold values of each cluster for both treatments can be found below:

_**VEH Threshold Values**_
<a href="url"><img src="https://github.com/pelinozsezer/RGS14/blob/main/nonrem_oscillations/Spectrograms%26GrangerCausality/vehicle_threshold_value_per_cluster.png" align="center" height="300" width="600" ></a>

_**RGS Threshold Values**_
<a href="url"><img src="https://github.com/pelinozsezer/RGS14/blob/main/nonrem_oscillations/Spectrograms%26GrangerCausality/rgs_threshold_value_per_cluster.png" align="center" height="300" width="600" ></a>
