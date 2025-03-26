# VHE_data_analysis_UB

During the hands-on on very-high-energy gamma-ray data we will see an example of a data analysis which you can follow and reproduce during the session and/or explore in more detail after that. You can try installing the required softwares on your own beforehand, using the below instructions. During the first session we will also do it together and try to solve any problems you encountered.

## Install of conda, gammapy and the git repository

### On Windows

Open a Windows PowerShell. Move to a location where you want to put miniconda (avoid spaces in the name of directories because the software does not like this). First we install miniconda (this will take a moment):
```
wget "https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe" -outfile ".\miniconda.exe"
Start-Process -FilePath ".\miniconda.exe" -ArgumentList "/S" -Wait
del .\miniconda.exe
```
Download the repository as follows: On the main page of the repository, in the top right of the webpage, press CODE (green button) and click the "Download ZIP" option at the bottom of the pop-up options. Move the zip file to the desired location on your PC and decompress it. Open an Anaconda PowerShell terminal and `cd` to the VHE_data_analysis_UB directory (probably you also have to do `conda deactivate` because the base environment is activated by default). Then, execute the following commands one after the other:
```
conda env create -f gammapy-1.3-environment_windows.yml
conda activate gammapy-1.3
```
Try to type `jupyter notebook` now, to see if you can open the notebooks in your browser.

### On linux/macOS

Open a terminal. Create a directory for the software in your home directory (indicated with ~):
```
mkdir -p ~/miniconda3
```
On linux download the installer with:
```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
```
on macOS instead with:
```
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh -o ~/miniconda3/miniconda.sh
```
Then execute:
```
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
source ~/miniconda3/bin/activate
conda init --all
```
Now `cd` to the location you choose for the git repository and do
```
git clone https://github.com/mpihet/VHE_data_analysis_UB.git
cd VHE_data_analysis_UB
```
Create a conda environment for the project with
```
conda env create -f gammapy-1.3-environment.yml
conda activate gammapy-1.3
```
Try to type `jupyter notebook` now, to see if you can open the notebooks in your browser.

## The git repository changed since you downloaded it?

### On Windows

Download the repository again, using the instructions above, or just download the missing files (the new notebooks) and save them in the VHE_data_analysis_UB directory on your PC.

### On linux/macOS

`cd` to the location of the cloned git repository and do `git pull`. If your local repository is not up to date with the remote git repository it should then update any changes.