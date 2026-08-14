#### Steps to run the case 

1) Open the run directory as per your console using the command: cd $FOAM_RUN
2) Then direct to the case file using the command: cd <casefilename>
3) run command : `blockMesh` to create and mesh the geometry from the blockMeshDict 

After successfully running the blockMesh command enter the next command 
4) run command : `buoyantPimpleFoam` to solve as per the boundry conditions and the initial values provided

After running the above command the simulation will start to run, after completion type 
5) run command : `paraFoam` to open paraFoam for viewing the results


Note: Some Allrun files may not work with every OpenFOAM version. If you encounter issues, follow the commands above. Otherwise:

1) run command: `./Allrun` to run all the commands automatically

After running the above command the simulation will start to run, after completion type 
2) run command : `paraFoam` to visualize and post-process


#### Common errors

If you encounter any floating-point errors during the case run, try reducing the deltaT in the system folder. This will help keep the maximum Courant number under 1.

If you experience other errors, check the version of OpenFOAM you're using, as it may differ from the version the case was originally set up for. You can also visit the CFD portal to find solutions.
