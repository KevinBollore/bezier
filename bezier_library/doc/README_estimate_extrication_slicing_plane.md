[![Institut Maupertuis logo](https://avatars1.githubusercontent.com/u/12760694?v=3&s=80)](http://www.institutmaupertuis.fr) 
estimateExtricationSlicingPlane function
=============================

This function is used too find number of lines which will be used to generate our extrication trajectories along the dilated mesh. By the same behavior than 
[estimateGrindingSlicingPlanes](README_estimate_grinding_slicing_planes.md) function, it will find a plan equation to cut the mesh in order to generate poses on resulting line.

To find one extrication equation, this algorithm find the last point of current grinding line n and the first point of next grinding line. It defines a triangle with this line, and the line defined by the last point of current line n and the same point with an offset which is following the global normal direction.

These lines create a triangle, which is need to define the plan equation which will cut the dilated mesh.
