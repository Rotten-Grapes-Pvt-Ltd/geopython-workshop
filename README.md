# Doing Geospatial Analysis in Python

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Rotten-Grapes-Pvt-Ltd/geopython-workshop/HEAD)

## ❓ What to expect out of this workshop.
This workshop will teach you about various python tools that will enable you to perform geospatial operations, either with existing data or by creating new datasets on the fly.
The purpose is to get familiar with most widely used python packages such as 
- pandas
- geopandas
- numpy
- matplotlib
- ipyleaflet
- mapdeck 
- GDAL/OGR,etc.
  
*we'll keep on updating this list and workshop in the future as well.

## 📚 What is the structure of workshop 

1. Understaning GIS 
2. Vector Data Analysis
3. Raster Data Analysis
4. Data visualisation


## Installation
For local installation of the code, perform the following steps 
### Environment setup (windows)
To set up a Python environment for your workshop on a Windows machine, you can use Micromamba, which is a lightweight package manager. Here's a step-by-step guide to setup

1. **Download Micromamba**: Execute the command in PowerShell. This will download the latest version of Micromamba.
```
Invoke-Webrequest -URI https://micro.mamba.pm/api/micromamba/win-64/latest -OutFile micromamba.tar.bz2
``` 

2. **Extract and Move Executable**: Unpack the micromamba.tar.bz2 file and move the micromamba.exe file to the root directory using the command 
```
MOVE -Force micromamba\Library\bin\micromamba.exe micromamba.exe
```

3. **Set Environment Variable**: Define the Mamba root prefix with 
```
$Env:MAMBA_ROOT_PREFIX="$HOME\micromambaenv"
```

4. **Invoke the Hook**: Run to invoke the necessary shell hook.
```
.\micromamba.exe shell hook -s powershell | Out-String | Invoke-Expression
```

5. **Initialize Shell**: Finally, initialize the shell with the command 
```
.\micromamba.exe shell init -s powershell -p "$HOME\micromambaenv"
```

6. **Create environment**: Create micromamba python environment from yaml file and activate
Go to your geopython-workshop repository and locate environment.yaml file is present and then run the command

```
micromamba env create -f environment.yaml
micromamba activate geoenv
```

With mamba or conda (if already installed)
```
mamba env create -f environment.yaml
```

### Environment setup (linux)

```
python3 -m venv .venv
source .venv/bin/activate
sudo apt-get -y install < apt.txt
pip install -r requirements.txt
```


## 👥 Who should attend this workshop ?
This workshop is meant for people who are work with [GIS](https://en.wikipedia.org/wiki/Geographic_Information_System). Their work includes things such as cleaning data, analysing data, processing data and with AI, also predicting data.
Anyone who is dealing in this can attend the workshop. 



