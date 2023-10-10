# LyonCutting_MNE_2023

MNE python tutorial - Lyon CuttingGardens 2023

## Material for the MNE-Python tutorial of Cutting Gardens 2023 - Lyon

More information Lyon Cutting Gardens [https://cuttinggardens2023.org/lyon](https://cuttinggardens2023.org/lyon)

Parts of these tutorials were first introduced in the 2022 Practical MEEG workshop: [http://practicalmeeg2022.org/](http://practicalmeeg2022.org/) and based on this fork: [https://github.com/Lx37/mne_pratical_meeg_2022](https://github.com/Lx37/mne_pratical_meeg_2022)

Authors of the material:

	- Britta Westner, Radboud University Nijmegen, Donders Institute
	- Alexandre Gramfort, Inria, CEA Neurospin
	- Denis A. Engemann, Inria, CEA Neurospin
  - Anne CHEYLUS, CNRS, CRNL
  - Romain Quentin, INSERM, CRNL
  - Pauline MOUCHES, CRNL

## Before you arrive

Please make sure you do the following steps before the first hands-on session:

1. If the username/login of your computer account has spaces and/or weird symbols, **YOU MUST** create a new user with a simpler name (no spaces, no symbols). Login with such a user name.
2. You will need to [download this directory](https://github.com/crnl-lab/mne_lyon_garden_2023/archive/refs/heads/main.zip) of scripts.
3. You will need to have an up-to-date python environment (3.11) and the latest version of MNE-Python (>=1.5.0) installed on your machine.

   If you're not familiar with python, we recommand to dowload Anaconda https://www.anaconda.com/download.
   We prepared a 'yaml' file, with all the python packages necessary for the tutorial.
   Once Anaconda is installed, launch it and go the 'environement' onglet. Import the environment 'Env_CuttingLyon_MNE.yml' and wait. This will create a new environment and install all the python packages.

   If you're familiar with python envs, you can pip install the the necessary packages :
 (you need a *full install* with all dependencies, **not** "MNE-Python with core functionalities only"). See instructions at: https://mne.tools/stable/install
```
pip install --upgrade pip
pip install mne
pip install PyQt5
pip install -U scikit-learn
pip install pandas
pip install jupyter
pip install mne-bids
pip install openneuro-py
```
4. You will need to download the data. Use this link [https://filesender.renater.fr/?s=download&token=2e2f23b0-24b8-4c60-8413-d838396ac562](https://filesender.renater.fr/?s=download&token=2e2f23b0-24b8-4c60-8413-d838396ac562). Place and unzip the data inside the scripts folder.
5. To check your installation, please look at the (very short!) notebook [Check your installation](0-Installation_check.ipynb). See below if you need a reminder how to start it.
6. For a full HD experience, we recommand that you read this [Short task explanation](Short_task_explanation.pdf).
7. If you are not familiar with Python, we invite you to take the time to work on these tutorials:
[Intro to Python](intro_to_python/0a-Intro_Python.ipynb), [Intro to Numpy](intro_to_python/0b-Intro_Numpy.ipynb).

### Activate your environement and Start a Jupyter notebook

Open your terminal (or an 'Anaconda Prompt') and navigate to the directory where you saved this directory of scripts.

To activate the tutorial environment, type the command `conda activate Env_CuttingLyon_MNE` (or the name of your python environment)

Then, to start a Jupyter notebook, type the command `jupyter-lab`. Jupyter should open in your internet browser. Click on the notebook you want to run!


## Program

#### Wednesday October 18, 2023

 - 09:00 – 10:30 MNE introduction [Preprocessing](1-Preprocessing.ipynb) 
 - 10:30 – 11:00 Break
 - 11:00 – 13:00 MNE decoding [Decoding](2-Decoding.ipynb)



### References and credit

The code from this tutorial is heavily inspired from this article:

	Mainak Jas, Eric Larson, Denis Engemann, Jaakko Leppakangas, Samu Taulu, Matti Hamalainen,
	and Alexandre Gramfort. 2018. A Reproducible MEG/EEG Group Study With the MNE Software:
	Recommendations, Quality Assessments, and Good Practices.
	Frontiers in Neuroscience. 12, doi: 10.3389/fnins.2018.00530

The MNE software when used in publications should be acknowledged using citations.

To cite MNE-C or the inverse imaging implementations provided by the MNE software, please use:

	A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck, L. Parkkonen,
	M. Hämäläinen, MNE software for processing MEG and EEG data, NeuroImage, Volume 86,
	1 February 2014, Pages 446-460, ISSN 1053-8119.

To cite the MNE-Python package, please use:

	A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck, R. Goj, M. Jas,
	T. Brooks, L. Parkkonen, M. Hämäläinen, MEG and EEG data analysis with MNE-Python,
	Frontiers in Neuroscience, Volume 7, 2013, ISSN 1662-453X.

The data processed in this tutorial was published with this article:

    R. Quentin, J-R. King, E. Sallard, N. Fishman, R. Thompson, E. Buch and L. Cohen (2020). 
    Differential brain mechanisms of selection and maintenance of information during working 
    memory (MEG data). OpenNeuro. [Dataset] doi: 10.18112/openneuro.ds002550.v1.0.1
