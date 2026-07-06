# CV
description of my work
# Taha Emad

**Biomedical engineer working at the intersection of clinical imaging hardware and applied machine learning.**

I've calibrated MRI, CT and PET-CT scanners on NHS floors *and* build deep-learning imaging models end to end a combination most ML engineers and most clinical engineers only have one half of. Currently completing an MSc in Healthcare Technologies at King's College London.

📍 London, UK  Tahaemad05@gmail.com 



## What I work on

Medical AI and imaging: turning MRI, CT and ultrasound data into robust, interpretable models with an eye on the DICOM, regulatory ISO 13485 and deployment realities that come from having worked on the hardware itself.

**Core stack:** Python · PyTorch · NumPy / Pandas / scikit learn · MATLAB · C
**Methods:** CNNs · graph neural networks · latent diffusion (VAE / DDPM) · Bayesian uncertainty · segmentation · spectral / dimensionality-reduction methods



## Featured projects

### 🧠 Prematurity classification from structural connectivity
graph based ML that predicts premature birth from diffusion MRI connectomes.

- **Problem:** classify preterm birth from 90×90 structural connectivity matrices small, noisy class imbalanced clinical data.
- **Approach:** reproducible Python pipeline with spectral graph embedding for dimensionality reduction ahead of classification; methods chosen for robustness to class imbalance.
- **Result:** **91% balanced accuracy** on a held out test set.
- **Stack:** Python · scikit-learn · graph methods

### 🌊 Neonatal Brain MRI synthesis age conditioned latent diffusion
A generative model that synthesises neonatal brain MRI slices at arbitrary gestational ages.

- **Problem:** generate anatomically plausible brain MRI slices conditioned on gestational age.
- **Approach:** built the full pipeline from scratch in PyTorch — a custom **VAE** (MSE + KL + patch adversarial loss) and an age conditioned **UNet DDPM** running in latent space, implementing the complete forward/reverse diffusion process.
- **Evaluation:** trained a CNN brain age regressor on 800 dHCP samples (target MAE < 1 week).
- **Stack:** PyTorch · diffusion models · VAEs

### 🫁 3D Lung Tumour Segmentation with Bayesian Uncertainty
Volumetric segmentation that also tells you how confident it is.

- **Problem:** segment small lung lesions in 3D under severe foreground/background class imbalance and GPU memory limits.
- **Approach:** 3D HighResNet with patch-based + hard region sampling and Generalised Dice loss; aleatoric/epistemic uncertainty via Bayesian methods; five-model ensemble.
- **Output:** IEEE conference format report.
- **Stack:** PyTorch · 3D CNNs · Bayesian deep learning

### 🔬 MSc Dissertation Multi-Transducer Ultrasound Elastography Phantoms
Designing tissue mimicking phantoms to validate an emerging imaging technique.

- Scoping an end to end validation project (literature review → requirements → fabrication → testing) for shear wave elastography on a multi transducer configuration, combining MATLAB modelling, 3D printing and bench top acoustic characterisation.



## Background

- **Field Imaging Engineer, Siemens Healthineers** — 30+ preventive maintenance cycles on CT / MRI / PET-CT across NHS sites; DICOM, ISO 13485, hands on imaging hardware.
- **BEng Biomedical Engineering**, University of Hull · **MSc Healthcare Technologies**, King's College London.
- interational level swimmer (Egypt) — 3rd, Open Water 5 km; 2nd, National 200 m Freestyle.
