[![Institut Maupertuis logo](https://avatars1.githubusercontent.com/u/12760694?v=3&s=80)](http://www.institutmaupertuis.fr) 
estimateExtricationSlicingPlane function
=============================

This function is used too find number of lines which will be used to generate our trajectories along the mesh. First, it will compute the number of plans which is necessary to cut mesh, following parameters. It finds bounds of mesh, and compute number of lines, depending on tool width and covering percentage.

![mesh_slicing](mesh_slicing.png)

When the number of lines is computed, we compute the offset of each line on the mesh (distance between lines has to be equal). In order to cut the mesh, we have to find planes equations. These plans equations (a.X + b.Y + c.Z + d = 0) are stored with slicing orientation vector and offset.
