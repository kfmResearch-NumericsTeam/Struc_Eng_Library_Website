# StrucEngLib Server

The StrucEng Library features a server component to run FEA solvers on a remote host.
This simplifies configuration setup and increases execution speed as FEA computations are remotely executed.

## Running StrucEngLib Server

On ibkpika host, start the server component by executing the file:
```
C:\Program Files\struc_eng_library\strucenglib_server\strucenglib_run_server
```
![image](https://user-images.githubusercontent.com/2311941/206233785-f8bceeaa-f334-497e-8f07-a1c96588aa17.png)

Upon successful launch, the server log shows current request and console output.

- During development phase of server, ensure to stop the server once you no longer make requests
(cancel server log window).

## Connecting with StrucEngLibrary Plugin
In Rhino 3D, ensure to have strucenglib plugin version 0.0.13 or later installed. If you are updating to version 0.0.13, ensure to re-run `StrucEnglibInstallDependencies` command in Rhino to update all Python dependencies.

### Enable Remote Computations
 Select _Execute on Server_ and inspect or execute model. The FEA computation will then be executed on remote server.
 
![image](https://user-images.githubusercontent.com/2311941/206236821-20bd1d30-06cb-4fd0-94b9-c9b5c9c90b4d.png)


## Source Code
The server component is hosted on [Github](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Server).
