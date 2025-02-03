# FDF
The program simulates values datasets that demos the software.

This program was run in Windows 64bit Windows 11. It should run on Linux and MAC and earlier versions of Windows as long as Java and Eclipse are installed but this has not been tested. The install time should take a few minutes.

For the Fire-Diffuse-Fire (FDF) agent based modeling, after saving the zip file and having it properly installed (preferably with Eclipse), choose the directory "examples", followed by "BSimChemicalFieldTest".

For installation instructions follow the eclipse guide README file. But it should be straightforward if Eclipse and the /zip file is installed.
1.     Click File -> Import  from the Eclipse main menu

2.     Expand General, select Existing Projects into Workspace, and click Next

3.     Make sure that Select Archive File is checked and browse for the ZIP file

4.     Click Finish

After this, download and install BSim from Github. https://github.com/CellSimulationLabs/bsim.git

Copy and Paste BSimChemicalFieldTest from this github into the eclipse workspace.

In this repository, there is a lot of different models for the FDF. For the standard FDF ABM used in the simulations, use the simple "BSimChemicalFieldTest"

Choose to preview or export the data in the last command lines by commenting "//" over the option you do not want to run. The data will be available in the directory "results2" if the export is chosen. Click run.

In line 317, choose totchem for the total amount of chemical in the whole system. Otherwise choose intensities for the average intensities (averaged in spherical shells at the line point). By choosing, this means to change the "totchem" to "intensities" or leaving it like so.  

The expected output for this FDF ABM if the preview option is chosen is a sphere of cells with a chemical field emanating from the center and the FDF. The run time per time step should be less than a second.

If totchem is chosen, the results2 directory should now contain a .csv file with the name specified on line 229, with a column of the timesteps and intensities. If intensities is chosen, the averaged intensity at each point on a line running in the "z" axes at each time interval should be displayed. This 
The run time should be half a second per timestep for a normal desktop computer or perhaps faster.



