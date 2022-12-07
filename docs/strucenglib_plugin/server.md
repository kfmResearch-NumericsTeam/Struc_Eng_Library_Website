# StrucEngLib Server

The StrucEng Library features a server component to run FEA solvers on a remote host.
This simplifies the configuration setup as there is no requirement to have an FEA solver locally installed.

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
In Rhino 3D, ensure to have strucenglib plugin version 0.0.13 or later installed.

## Source Code
The server component is hosted on [Github](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Server).
