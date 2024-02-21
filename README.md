# Automatic Extraction of Speech Biomarkers for the Early Diagnosis of Neurocognitive Disorder

## Table of Contents
+ [About](#about)
+ [Materials](#materials)
+ [Demo](#examples)


## About <a name = "about"></a>
This repository provides additional materials for the final project of the Digital Humanities & Digital Knowledge Master Degree, that included the development of a python package designed for processing audio files and extracting acoustic biomarkers for the identification of neurocognitive disorder from speech. The objective of the work is to contribute to current research in the identification of linguistical manifestations of the illness, towards the creation of reliable and non-intrusive tools for its early detection.

 ## Materials

The Notebooks directory contains the following materials:
- **Voice Activity Detection (VAD) Evaluation**
- **Package demonstration**
<!--- **Temporal speech parameters:** mean, median and standard deviation of speech and silence segments, percentage on silence ratio, percentage on silence to speech ratio, transformed phonation rate.

- **Pitch related:** F0 (Sub-Harmonic-Summation & Post-Viterbi Smoothing)

- **Spectral features:** MFCC, Spectral descriptors and moments (Spectral centroid, skewness, variance, flux) and formants (F1-F3)

- **Voice Quality:** Shimmer, Jitter, Harmonics to Noise Ratio

- **Self-similarity:** Complexity of the speech signal using the Higuchi Fractal Dimension Algorithm. -->

 <!-- Please refer to the <a href="#details"> details </a> section for more. -->
<!--
### Prerequisites

This program has been developed and tested on Linux (Ubuntu) environment. -->

<!-- ### Installing/Requirements

Clone the repository and install the necessary packages with the install_requirements.sh inside the project's directory.

```
# if on colab
!git clone https://github.com/chloeppd/AcousticDLBextractor

%cd AcousticDLBExtractor

!bash install_requirements.sh
```

You may also need to get the necessary permissions:
```
!chmod 755 -R /content/AcousticDLBextractor
``` -->





## Demo <a name = "examples"></a>

See a demonstration of the package using samples from the <a href="http://www.clips.unina.it/it/index.jsp">CLIPS</a> corpus on the Google Colab Notebook.

<a target="_blank" href="https://github.com/chloeppd/MasterThesisDHDK/blob/main/Notebooks/demo.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>



<!--## Details and Acknowledgments<a name = "details"></a>



- This project uses the **INTERSPEECH 2016 ComparE and GeMAPS feature sets** using the <a href="https://github.com/audeering/opensmile-python?tab=readme-ov-file">openSMILE</a> python wrapper for audio analysis.

- **Voice Activity Detection** is performed using <a href="https://github.com/enmwmak/ssvad">SS-VAD</a> Voice Activity Detector for NIST Speaker Recognition Evaluation by Mak & Yu.

- **The Higuchi Fractal Dimension Algorithm** is retrieved from <a href="https://github.com/inuritdino/HiguchiFractalDimension">this package</a> at master commit: fef4903.

- **The sample audios** are from the open access <a href="http://www.clips.unina.it/it/index.jsp">CLIPS</a> corpus (Corpora e Lessici dell'Italiano Parlato e Scritto). -->
