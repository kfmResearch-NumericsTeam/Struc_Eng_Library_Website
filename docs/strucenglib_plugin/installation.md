The easiest way to install StrucEngLibrary Plugin is with Rhino's Package Manager. 

## Rhino Package Manager  <small>recommended</small>
Type `PackageManager` in Rhino command line and search for `StrucEngLibPlugin`
in the search bar. Select the latest version, then hit install, and restart
Rhino.

<figure markdown>
  ![](assets/install.png)
  <figcaption>Rhino Package Manager</figcaption>
</figure>



!!! note
    - For a list of recent changes, see the [changelog](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library_Plug_in/blob/master/CHANGELOG). 
    - If you are interested in developer builds, enable `Include pre-releases`.


## Menu bar and Command integration
Upon restart, the plugin integrates into Rhino menu bar and is accessible under `Tools` - `StrucEngLib Plugin` as well as in the command line with `StrucEngLib*`.

If plugin load fails with an error, ensure that the plugin is loaded `PluginManager` settings:
![image](https://user-images.githubusercontent.com/2311941/206239991-0800a332-0b85-4005-a3de-16ababcd698f.png)

## Post Installation
Upon installation of the plugin, various python dependencies must be downloaded.

!!! note
    - The installer will also install the latest versions of Compas and Compas FEA 1 from pip.


### Download code snippets

Type `StrucEngLibInstallDependencies` in Rhino command line to open the dialog shown below.

<figure markdown>
  ![](assets/installer.png){width=500px}
  <figcaption>StrucEng Library Dependency Installer</figcaption>
</figure>

For `Anaconda Home Directory` select your Anacoda installation directory from
[prerequisite step](../getting_started/#install-anacoda) and press `Install`.
The StrucEngLib Plugin will use anaconda to create a new virtual environment, and
install all required python depdencies. With `Test Import`, the python
dependencies can be checked. Upon failure, an error message is shown.

!!! note
    - The installer will use Compas to install python dependencies into Rhino's include directory `%AppData%\McNeel\Rhinoceros\7.0\scripts`. 
    - Compas/ Compas Fea no longer recommends to set `%PYTHONPATH%` variable. In case you still have it manually set, please undo.
    - If you changed Rhino's `Modules Search Path` in Python Editor, please remove them ([Why](https://web.archive.org/save/https://compas.dev/compas_fea/latest/gettingstarted/installation.html)) StrucEngLib Plugin installer will take care of python dependencies.
    - The dependency installer installs the [following dependencies](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library_Plug_in/blob/master/StrucEngLib/EmbeddedResources/install.bat).


 
