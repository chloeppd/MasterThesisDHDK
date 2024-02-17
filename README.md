#Automatic Extraction of Speech Biomarkers for the Early Diagnosis of Neurocognitive Disorder 

## Table of Contents
+ [About](#about)
+ [Usage - Examples](#examples)
+ [Details and Acknowledgments](#details)

## About <a name = "about"></a>
This repository provides additional materials for the final project of the Digital Humanities & Digital Knowledge Master Degree. A Python package was designed for processing audio files and extracting acoustic biomarkers for the identification of neurocognitive disorder from speech. Its objective is to contribute to current research in the identification of linguistical manifestations of the illness, and support the training of automatic classifiers with the scope to devise reliable and non-intrusive tools for the early detection of neurocognitive disorder through speech. 

<!-- ## Features

- **Temporal speech parameters:** mean, median and standard deviation of speech and silence segments, percentage on silence ratio, percentage on silence to speech ratio, transformed phonation rate.

- **Pitch related:** F0 (Sub-Harmonic-Summation & Post-Viterbi Smoothing)

- **Spectral features:** MFCC, Spectral descriptors and moments (Spectral centroid, skewness, variance, flux) and formants (F1-F3)

- **Voice Quality:** Shimmer, Jitter, Harmonics to Noise Ratio

- **Self-similarity:** Complexity of the speech signal using the Higuchi Fractal Dimension Algorithm. -->

 Please refer to the <a href="#details"> details </a> section for more.

### Prerequisites

This program has been developed and tested on Linux (Ubuntu) environment.

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




```
# demo
audio_processor = AudioProcessor('your_wav_file.wav')

# speech and silence segments
audio_processor.spe_sil_stats()

# return all features on a global utterance and file level (recommended for saving computation time)
file_level, segment_level = get_all_features(audio_processor,average="both")

```

## Usage-Examples <a name = "examples"></a>

See a demonstration on the Google Colab Notebook!

<a target="_blank" href="https://colab.research.google.com/github/chloeppd/AcousticDLBextractor/blob/main/Notebooks/demo.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>


## Details and Acknowledgments<a name = "details"></a>

- This project uses the **INTERSPEECH 2016 ComparE and GeMAPS feature sets** using the <a href="https://github.com/audeering/opensmile-python?tab=readme-ov-file">openSMILE</a> python wrapper for audio analysis.

- **Voice Activity Detection** is performed using <a href="https://github.com/enmwmak/ssvad">SS-VAD</a> Voice Activity Detector for NIST Speaker Recognition Evaluation by Mak & Yu.

- **The Higuchi Fractal Dimension Algorithm** is retrieved from <a href="https://github.com/inuritdino/HiguchiFractalDimension">this package</a> at master commit: fef4903.

- **The sample audios** are from the open access <a href="http://www.clips.unina.it/it/index.jsp">CLIPS</a> corpus (Corpora e Lessici dell'Italiano Parlato e Scritto).
