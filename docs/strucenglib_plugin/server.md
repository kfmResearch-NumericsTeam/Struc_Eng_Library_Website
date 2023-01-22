# StrucEngLib Server

The StrucEng Library features a server component to run FEA solvers on a remote host.
This simplifies configuration setup and increases execution speed as FEA computations are remotely executed.

## Running StrucEngLib Server
A server instance is deployed on ibkpika host. When connected to ETH network, browse [http://ibkpika.ethz.ch:8080/](http://ibkpika.ethz.ch:8080/) to access the server log.

[
![image](https://user-images.githubusercontent.com/2311941/213932152-da7c3f7e-8d11-403d-b5a7-00c9f6040f9a.png)](http://ibkpika.ethz.ch:8080/)

The server log shows remote computation status logs. You may access the log during remote computations to keep track of computation results.

## Connecting with StrucEngLibrary Plugin
In Rhino 3D, ensure to have strucenglib plugin version 0.0.13 or later installed. If you are updating to version 0.0.13, ensure to re-run `StrucEnglibInstallDependencies` command in Rhino to update all Python dependencies.

### Enable Remote Computations
 Select _Execute on Remote Server_ and inspect or execute model. The FEA computation will then be executed on remote server.
 
 ![image](https://user-images.githubusercontent.com/2311941/206236821-20bd1d30-06cb-4fd0-94b9-c9b5c9c90b4d.png)

Remote computations outsorce Compas FEA `analyse_and_extract` invocations to the server.

```python
# Run on Sever ws://ibkpika.ethz.ch:8080
mdl = connect.analyse_and_extract('ws://ibkpika.ethz.ch:8080/api/compute', mdl, software='abaqus', fields=[  ] )

```

## Source Code
The server component is hosted on [Github](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Server).

