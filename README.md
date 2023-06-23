# Eikonal Model

- This Python code implements the eikonal model to compute the spatial organization of planar hillslopes bounded at a threshold angle.
- The results obtained using this model have been tested for accuracy in diverse geologic settings and hydroclimatic conditions.
- In terms of data requirement, the model needs solely the shape of the boundary enclosing the landscape to produce the topography.
  
# Installation

- The code is presented as a *jupyter notebook*, which can be installed using pip as `pip install notebook` or using Conda `conda install -c conda-forge notebook`.
- Required Python libraries are *numpy* *shapely* libraries, which can be installed using pip as `pip install numpy` and `pip install shapely`, respectively. 
- The jupyter notebook also uses the *matplotlib* library, which can be installed as `conda install -c conda-forge matplotlib` or using Conda `python -m pip install -U matplotlib`.
- File **Downstream_Boundary.npy** (2 \times N) in the repository is the array used as the x and y coordinates of the enclosing boundary.

# Code structure

Each number written in the list below explains the operations and functions for the particular Cell of the Jupyter Notebook.
1. Import relevant packages from the above-mentioned libraries.
2. Define the Python function for computing the erosion term implicitly using the D_infinity flow direction method and also define the Python function that updates the diffusion term implicitly using the LGMRES algorithm. 
3. Initializing the coefficients, domain size, and model parameters to be used in the solver.
4. Initializing the raster grid, boundary conditions, and the initial condition for the simulation run.
5. *While* loop for the simulation run until the steady-state is reached.
9. Save the elevation and drainage area arrays for plotting and further investigations.

# Contact Us

For more information about this research, you can reach out to me: [Shashank Kumar Anand](mailto:skanannd@princeton.edu?subject=[GitHub]%20Landscape%20Evolution%20Model%20(LEM)%20Numerical%20Solver). 
