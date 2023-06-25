# Eikonal Model

- This Python code implements the eikonal model to compute the spatial organization of planar hillslopes bounded at a threshold angle.
- The results obtained using this model have been tested for accuracy in diverse geologic settings and hydroclimatic conditions.
- In terms of data requirement, the model needs solely the shape of the boundary enclosing the landscape to produce the topography.
  
# Installation

- The code is presented as a *jupyter notebook*, which can be installed using pip as `pip install notebook` or using Conda `conda install -c conda-forge notebook`.
- Required Python libraries are *numpy* *shapely* libraries, which can be installed using pip as `pip install numpy` and `pip install shapely`, respectively. 
- The jupyter notebook also uses the *matplotlib* library, which can be installed as `conda install -c conda-forge matplotlib` or using Conda `python -m pip install -U matplotlib`.

# Input
- A file providing the boundary condition for the model. As an example, file **Downstream_Boundary.npy** in the current repository is the 2D array that provides the *x* and *y* coordinates of the enclosing boundary.

# Code structure

Each number in the list below explains the operations and functions of the particular cell in the Jupyter Notebook.
1. Import relevant packages from the libraries mentioned above.
2. Get the input boundary (*x* and *y* coordinates), threshold angle, and the raster resolution. 
3. Initialize the shapely polygon based on the boundary given and plot it.
4+5. Use the defined polygon to create the eikonal topography and visualize it.
6. Fill the elevation field outside the boundary with null values and visualize the final eikonal topography.

# Contact Us

For more information about this research, you can reach out to me: [Shashank Kumar Anand](mailto:skanannd@princeton.edu?subject=[GitHub]%20Landscape%20Evolution%20Model%20(LEM)%20Numerical%20Solver). 
