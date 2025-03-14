# CHD Adversarial NN
## An Adversarial Framework for Mitigating Gender Bias in Coronary Heart Disease Prediction.

| Spec | Details |
| --- | --- |
| Group ID | Group A10-2 |
| Authors | Diego Silva (d1silva@ucsd.edu), Patrick Salsbury (psalsbury@ucsd.edu), Kai Ni (c5ni@ucsd.edu) |
| Mentors | Emily Ramond (eramond@deloitte.com), Greg Thein (gthein@deloitte.com) |
| Project Site | <https://chd-adversarial-nn.github.io> |

## How to Get Started
Follow the instructions listed on this page to set up and replicate our project on your local environment.

## 1) Cloning Code
- Clone repository into your working directory:
    `git clone https://github.com/patsals/DSC-180-Capstone.git`
- Enter the repository directory `DSC-180-Capstone`

## 2.a) Setting up Environment (Windows Users)
- Install Linux using Windows Subsystem for Linux (WSL) in powershell:
    `wsl --install`
- Install Linux Distribution System through Microsoft store:
    `Ubuntu 22.04.5 LTS`
- Open Ubuntu and wait for download to complete
- Once download complete enter a Username and Password as prompted
- Open VS Code then click on the two caret mark icon on the bottom left of window:
- Select the "Connect to WSL Using Distro..."
- You should see `Ubuntu 22.04.5 LTS` and select that option
- Proceed to 2.b instructions

## 2.b) Setting up Environment (Linux/Mac OS users)
- Note: TensorFlow may not be available for the latest version of Python. As of the development of this project, we are using Python 3.11.
- Create a working environment:
    `python3 -m venv venv`
- Activate the working environment:
    `source venv/bin/activate`
- Download the dependencies:
    `pip install -r requirements.txt`

## 3) Downloading & Processing Data
- Run the data setup script to extract, transform, and load all of the data locally:
    - `python data_setup.py` for windows users
    - `python3 data_setup.py` for Linux/Mac OS users
    - adding the `--skip_download` flag skips the requesting/downloading of files
- Run the data processing script to handle null/missing values:
    - `python data_process.py` for windows users
    - `python3 data_process.py` for Linux/Mac OS users
- Note: The setup script makes requests to multiple url endpoints at www.sciencedirect.com to download the files. It is important to lookout for any message logs that do not show `[SUCCESS]` as an output — this indicates an error that needs to be resolved.
