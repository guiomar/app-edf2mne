# app-edf2mne

<!-- brainlife-app:begin (generated from the App manifest; edit the manifest, not this block) -->

> **Converts an EEG recording in EDF format to MNE-Python Raw (.fif) with mne.io.read_raw_edf.**

Utility that reads the EDF file of an EEG dataset with MNE-Python and saves it as raw.fif so it can be used by brainlife MNE Apps. Only the EDF data file is converted; the BIDS channels, electrodes, coordinate system and events sidecars of the input are not applied.

| | |
|---|---|
| 📥 **Inputs** | `neuro/eeg/edf` |
| 📤 **Outputs** | `neuro/meeg/mne/raw` |
| 🐳 **Container** | `brainlife/mne:0.23dev` |
| ⚙️ **Resources** | 8 CPUs |
| 🔗 **Run it** | [doi.org/10.25663/brainlife.app.637](https://doi.org/10.25663/brainlife.app.637) |

#### 📥 Inputs

| Input | Datatype | Required | Description |
|---|---|---|---|
| `edf1` | `neuro/eeg/edf` | yes | EEG recording in EDF format with optional BIDS sidecars (channels, electrodes, coordsystem, events). |

#### 📤 Outputs

| Output | Datatype | Description |
|---|---|---|
| `out_dir` | `neuro/meeg/mne/raw` | MNE Raw data in FIF format |

📚 **References used by this App:**
- Hayashi S., Caron B. A. et al. brainlife.io: A decentralized and open source cloud platform to support neuroscience research. arXiv (2023).
- Gramfort A. et al. MEG and EEG data analysis with MNE-Python. Frontiers in Neuroscience 7:267 (2013). [doi:10.3389/fnins.2013.00267](https://doi.org/10.3389/fnins.2013.00267)

<!-- brainlife-app:end -->

[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/brain-life/abcd-spec)
[![Run on Brainlife.io](https://img.shields.io/badge/Brainlife-bl.app.637-blue.svg)](https://doi.org/10.25663/brainlife.app.637)

## Documentation
Converts EEG `edf` files to MNE raw data, using `mne.io.read_raw_edf` function from MNE-python.

1) Input file is:
    * `eeg/edf` meg data file
2) Ouput files are:
    * `meeg/mne/raw` eeg raw.fif data file

## Authors
- [Guiomar Niso](guiomar.niso@ctb.upm.es), Instituto Cajal, CSIC, Spain

## Citations
We kindly ask that you cite the following articles when publishing papers and code using this app. 

1. **brainlife. io: A decentralized and open source cloud platform to support neuroscience research**. Hayashi, S., Caron, B. A., et al. & Pestilli, F. (2023). ArXiv. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10274934/

2. **MEG and EEG data analysis with MNE-Python**. Gramfort A, et al. & Hämäläinen MS. (2013). Frontiers in Neuroscience, 7(267):1–13, 2013. https://doi.org/10.3389/fnins.2013.00267

## Funding Acknowledgement
brainlife.io is publicly funded and for the sustainability of the project we kindly ask that you acknowledge the following funding sources:

[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)
[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)
[![NSF-ACI-1916518](https://img.shields.io/badge/NSF_ACI-1916518-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1916518)
[![NSF-IIS-1912270](https://img.shields.io/badge/NSF_IIS-1912270-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1912270)
[![NIH-NIBIB-R01EB030896](https://img.shields.io/badge/NIH_NIBIB-R01EB030896-green.svg)](https://grantome.com/grant/NIH/R01-EB030896-01)


#### MIT Copyright (c) 2021 brainlife.io The University of Texas at Austin and Indiana University
