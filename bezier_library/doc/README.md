How to build the API documentation
==================================
```bash
cd $(catkin_workspace)/build
make bezier_library_doc
```

Goals
=====
Design a fully automated robotized grinding application

Functions
- F1: Being able to locate the part (different shapes, only coarse location is known, small batches)
- F2: Ensure a constant material removal rate (CAM)
- F3: Being able to respect the manufacturer's specifications (dimensions, manage tool wear)

Automatically grind defects on a mechanical part thanks to:
- A robot
- 3D vision

Defects types
- Shocks, deformations, welding spatters, weld bead ...
- Surface roughness

Numerical blocks
================
3D -> 3D sensor -> 3D scanning -> 3D metrology -> Robot path planning -> Grinding

How Bézier works
================

For surfacing mode, please see [bezier_grinding_surfacing](README_bezier_grinding_surfacing.md) documentation.
