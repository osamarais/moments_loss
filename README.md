# Moments Loss for 3d Reconstruction

This repository is an exploration of the efficacy of 3D moments used as a loss function for 3D shapes.

2D and 3D moments have been used for image and 3D object matching or similarity measuremet. They can be made 
invariant to scale, translation, and rotation.

Since moments are better at capturing the overall shape of objects in 2D or 3D, they can possibly serve as a 
better objective function for machine learning applications.

For 2D images the calcuation is straightforward using pixel values.

In 3D the object may be defined using voxels (which take binary values) or a surface mesh.
Calcuation over voxels is a straightforward extentsion from 2D pixel values.
For surface meshes the calcuation can be done efficiently with surface integrals.


The dataset targeted for this study is ShapeNet.

The surface meshes are loaded using the pymeshlab library.
This can easily be installed using
```
pip3 install pymeshlab
```
