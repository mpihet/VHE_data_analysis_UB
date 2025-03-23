# VHE_data_analysis_UB

## Preparation and Install of Software

During the hands-on on very-high-energy gamma-ray data we will see an example of a data analysis which you can follow and reproduce during the session and/or explore in more detail after that. You can try installing the required softwares on your own beforehand, using the below instructions. During the first session we will also do it together and try to solve any problems you encountered.

- You will need a distribution of [miniconda](https://www.anaconda.com/docs/getting-started/miniconda/install), which is installable following the instructions for the respective operating system you are using.

- Clone the repository

For Linux/macOS execute the following command from a terminal in a directory of your choice (`cd` to the location first):
```
git clone https://github.com/mpihet/VHE_data_analysis_UB.git
cd VHE_data_analysis_UB
```
On Windows download the repository as follows: On the main page of the repository, in the top right of the webpage, press CODE (green button) and click the "Download ZIP" option at the bottom of the pop-up options. Move the zip file to the desired location on your PC and decompress it. Open an Anaconda PowerShell terminal and `cd` to the TEFPA_gray_handson directory. 

- Create and activate the gammapy v1.3 environment

If you use Windows, use (once inside the VHE_data_analysis_UB directory):
```
conda env create -f gammapy-1.3-environment_windows.yml
conda activate gammapy-1.3
```
Else, use:
```
conda env create -f gammapy-1.0-environment.yml
conda activate gammapy-1.3
```
Now you are ready to open the notebooks using the command `jupyter notebook` inside the terminal. It will open them inside a browser.
