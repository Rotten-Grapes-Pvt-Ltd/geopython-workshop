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
```.

4. **Invoke the Hook**: Run to invoke the necessary shell hook.
```
.\micromamba.exe shell hook -s powershell | Out-String | Invoke-Expression
```

5. **Initialize Shell**: Finally, initialize the shell with the command 
```
.\micromamba.exe shell init -s powershell -p "$HOME\micromambaenv"
```


### Environment setup (linux)

1. Download micromamba: 



6. **Create environment**: Create micromamba python environment from yaml file and activate
```
micromamba create -f environment.yaml -y
micromamba activate geoenv
```


### Reference:

https://mamba.readthedocs.io/en/latest/micromamba-installation.html#windows

## All Jupyter Notebook Assets

Jupyter Notebook is used to run all examples and exercises.

