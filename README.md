# dendro-contour
The dendrogram contouring project aims at providing a statistically sound tool to examine the distribution of various physical properties of structures at different scales.  The goal is to be able to identify the hierarchical structures in the molecular clouds and to derive the physical properties not only of the dendrogram features but also for regions/volumes defined by incrementally increasing density contours.

## Structure of the Project
The project is structured into a four-step process.  In the first step, the data are collected.  Acceptable data formats should include observations of column density and molecular line(s), simulated cube in the real (6D = PPP + Vx + Vy + Vz) space, and the synthetic observation of the simulations (again including the maps of column density and molecular line(s)).

In the second step, the dendrogram is run on the density map/cube.  The result should include a dictionary of masks associated with the dendrogram features.

In the thrid step, the masks from the second step is then used to define the regions/volumes for which physical properties are derived.

In the last step, the results are visualized as a color-coded tree diagram and as a color-coded contour map.  On the resulting tree diagram and the map, there should be an option to include other information including the YSO positions.  Scatter plots with connecting lines showing the dendrogram structure should also be available in cases where multiple properties are derived in step 3.

## About this Repo
This repo serves as the container of the data and the codes used in the analyses.  Near the end of the project, the repo may also contain drafts of the journal paper(s) generated from this project.

## To-do
1. Transfer the code from the [Dryads project](https://github.com/hopehhchen/Dryads) and make the code compatible with the simulation output in the real space.  (Mainly to make sure that the mask generating part works for both a 2D map and a 3D cube.)

2. Generate synthetic observations of the simulated cubes using [RADMC3-py](http://www.ita.uni-heidelberg.de/~dullemond/software/radmc-3d/).

### Credits and Contacts
The project is a collaboration between Hope Chen and Stella Offner at the University of Texas at Austin.  The project was initiated by Stella Offner and Chris Faesi.  In the future, several other ongoing projects, including a project aiming at tracking the dendrogram features throughout the evolution of a simulated cloud and another project focusing on the automatic identification of structures in simulations, may be linked to provide a bette platform for dendrogram-related projects to provide the context for each other.

Hope Chen is currently responsible for managing this GitHub repo.  He can be reached via email at hopechen@utexas.edu.
