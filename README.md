# 🧠 EEG Alpha Brain Activity Analysis Using Python

## 📌 Project Overview

This project explores brain activity using electroencephalography (EEG) data with a focus on **alpha wave (8–12 Hz) analysis**. The goal is to demonstrate how signal processing techniques can be used to extract meaningful neural rhythms and interpret brain states.

Using Python and the MNE library, raw EEG signals were processed, filtered, and transformed into the frequency domain to study alpha power distribution across different brain regions.

---

## 🎯 Objectives

- Load and explore real EEG dataset
- Preprocess raw EEG signals (noise reduction and filtering)
- Perform frequency-domain analysis using Power Spectral Density (PSD)
- Extract and quantify alpha band activity (8–12 Hz)
- Visualize spatial distribution of alpha power across EEG channels
- Interpret results in a neuroscience context

---

## 📊 Dataset

The EEG data used in this project is from the **EEG Motor Movement/Imagery Dataset** available on PhysioNet:

https://physionet.org/content/eegmmidb/1.0.0/

This dataset contains multichannel EEG recordings from human subjects under different resting and task conditions.

---

## 🛠️ Tools & Libraries

- Python
- NumPy
- Matplotlib
- MNE-Python (neurophysiological data analysis)

---

## 🔬 Methodology

### 1. Data Loading
Raw EEG signals were loaded using MNE’s built-in dataset loader and EDF reader.

### 2. Preprocessing
Signals were filtered using a bandpass filter (1–40 Hz) to remove:
- Slow signal drift
- High-frequency noise

### 3. Frequency Analysis
Power Spectral Density (PSD) was computed using the Welch method to convert time-domain EEG signals into frequency-domain representations.

### 4. Alpha Band Extraction
Alpha activity was isolated within the 8–12 Hz frequency range and averaged across channels to quantify brain rhythm strength.

### 5. Visualization
Alpha power distribution was plotted across EEG channels to observe spatial variation in brain activity.

---

## 📈 Key Findings

- Alpha activity was successfully isolated from raw EEG signals.
- There is clear variation in alpha power across different brain regions.
- This variation reflects functional differences in cortical activity.
- Higher alpha power is generally associated with relaxed or idle brain states.

---

## 🧠 Interpretation

Alpha waves (8–12 Hz) are strongly associated with relaxed wakefulness and reduced cognitive load.

In this analysis:
- Channels with higher alpha power suggest regions in a more inhibited or resting state.
- Lower alpha power indicates increased neural activity or engagement.

These findings are consistent with established neuroscience literature on alpha oscillations and cortical activity.

---

## 🚀 Project Upgrade (Advanced Extension)

To enhance the analysis, an additional comparison was performed:

### 🔄 Condition-Based Insight (Extended Idea)

The dataset structure allows comparison between different resting/task conditions (e.g., eyes open vs eyes closed or baseline vs task states).

In an extended version of this project, alpha power can be compared across conditions:

- **Eyes closed condition** → expected increase in alpha power  
- **Eyes open condition** → expected suppression of alpha activity  

This extension strengthens the biological interpretation of the results and moves the analysis closer to experimental neuroscience research standards.

---

## 📌 Limitations

- This analysis uses a simplified subset of EEG data
- No artifact removal (e.g., ICA) was applied in this version
- Channel-level interpretation is not source-localized
- Further work is needed for clinical or diagnostic conclusions

---

## 🔮 Future Work

- Apply Independent Component Analysis (ICA) for artifact removal
- Perform eye-open vs eye-closed condition comparison
- Extend analysis to theta and beta frequency bands
- Integrate machine learning for brain state classification
- Visualize topographic brain maps of alpha activity

---

## 👩🏽‍💻 Author

Built as part of a neuroscience signal processing learning project using Python.

---

## 📚 Acknowledgement

- PhysioNet EEG Motor Movement/Imagery Dataset
- MNE-Python documentation and community
