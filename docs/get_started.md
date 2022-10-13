# Get Started

## Prerequisites
### Rhino 7
StrucEng Lib is a Plugin for Rhino. Download a recent version of Rhino 7 from https://www.rhino3d.com/7/new/.  
ETH Zurich members can use [a floating license with Rhino Cloud Zoo](https://web.archive.org/web/20220701094920/https://gramaziokohler.arch.ethz.ch/teaching-materials/00_installation/1_rhino/) when connected with VPN.

Known working versions of Rhino include:
  - Version 7 SR19 or later

### Windows
This plugin runs on a recent version Microsoft Windows only (due to Abaqus).

## Install
### Via Rhino Package Manager
The easiest way to install StrucEngLibrary Plugin is with Rhino 7's Package Manager. Type `PackageManager` in Rhino Command line and search for `StrucEngLibPlugin` in the search bar.

Select the latest version, then Install, and restart Rhino.

[https://user-images.githubusercontent.com/2311941/172725314-50b9c44b-6e56-4fe9-98b7-8c7836ac4053.png|width=800px]

- If you are interested in developer builds, enable `Include pre-releases`.
- Ensure you have a recent Rhino Version installed as older versions cause issues with Rhino Panels.
- For a list of recent changes, browse [CHANGELOG](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library_Plug_in/blob/master/CHANGELOG) file in the root directory of the repository.

## Menubar Integration
Upon restart, StrucEngLib integrates into Rhino menubar and is accessible under Tools - StrucEngLib Plugin:

[[https://user-images.githubusercontent.com/2311941/172724767-9abfdd50-2c0e-4add-b97e-b559779f3c70.png|width=500px]]

The menubar is a visual shortcut for important command. All StrucEngLib Plugin Rhino commands are prefixed with `StrucEngLib*`:

[[https://user-images.githubusercontent.com/2311941/183244303-4a0b2f43-1477-47dc-b636-ad2f90b236ec.png|width=300px]]


## Post Installation Steps
Upon Installation of StrucEngLib Plugin, ensure you have all necessary Python dependencies installed.

### Install Python Dependencies 
StrucEngLib Plugin includes a dependency installer. Type command `StrucEngLibInstallDependencies` to open the dialog shown below:

[[https://user-images.githubusercontent.com/2311941/178495158-084905fd-e5df-4ed0-9be8-1f497a0a59d7.png|width=500px]]

- 1. Select the home directory of anaconda. If anaconda is not installed, it must be downloaded and installed first (i.e. press browse website, select [64-Bit Graphical Installer (594 MB)](https://repo.anaconda.com/archive/Anaconda3-2022.05-Windows-x86_64.exe) -> see installation proceedere in the next sections below).
- 2. Press Install, StrucEngLib Plugin will use conda to create a new virtual environment, and install compas, compas-fea and sandwichmodel.
- 3. With 'Test Import', the python dependencies can be checked. Upon failure, an error message is shown.
- The installer will use compas to install python dependencies into Rhino's include directory `%AppData%\McNeel\Rhinoceros\7.0\scripts` [See installer commands](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library_Plug_in/blob/master/StrucEngLib/EmbeddedResources/install.bat).
- Compas/ Compas Fea no longer recommends to set %PYTHONPATH% variable. Additionally, if you changed Rhino's Modules Search Path in Python Editor, please remove them [Source](https://compas.dev/compas_fea/latest/gettingstarted/installation.html). StrucEngLib Plugin installer will take care of python dependencies. 

### Required Python packages
All required python packages for the StrucEng Library are fundamental packeges and are installed during your python installation.

### Installation of Anaconda prompt
... coming soon ...

### Installation of Abaqus
Abaqus FEA is a software suite for finite element analysis and computer-aided engineering. Its installation cannot be automated.
For ETH Zurich members, order (free) a copy via IT shop: [Abaqus 2021](https://itshop.ethz.ch/)

- Follow installation instructions in IT shop:
  - Install: ..\AM_SIM_Abaqus_Extend.AllOS\1\setup.exe
  - License Server (ETH VPN): SIMULIA FLEXnet with License Server: 1973@lic-abaqus-teaching.ethz.ch

- [Installation guide (3rd party)](https://web.archive.org/web/20220718103200/https://deviceanalytics.com/install-abaqus-on-windows/)
