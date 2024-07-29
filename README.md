<div align="center">

[Overview](#Overview) -
[Features](#Features) -
[How to use it](#How-to-use-it) -
[Get Help](#Get-Help) -
[Copyright Notice](#copyright-notice) -
[License](#License) -
[Citation](#Citation)

</div>

## Overview

A new preprocessing toolkit is developed to generate accurate initial conditions 
for particle-method-based CFD simulations with complex geometries. The algorithm is 
based on the improved Marching Cubes method (MC) with the newly proposed isosurface 
particle redistribution optimisations.

## Features

- C++ implementation
- Support for particles
- Supporting various data sources such as volumetric images and common CAD models (e.g. STL files).
- Efficiently generate uniformly distributed internal fluid particles of any shape at no extra cost.
- Provides certain high-precision particle boundary conditions
- The iterative particle moving algorithm achieves and verifies a high-quality distribution for boundary particles on surface,
- Plotfile format supported by Tecplot and ParaView

## How to use it

We currently provide executables of the preprocessing algorithm programs containing implementations of 
the algorithms and test cases from the paper, as well as exact SDF scalar fields for more than 30 geometries 
as supplementary cases. The executables are generated in the window environment. New features of the 
preprocessing tool are currently being developed, so the full source code will be published in the future.

When running the executable file CMC33.exe, the following prompt will appear:
Which 3D complex particle flow field reconstruction algorithm do you want to choose, the CMC33, STL algorithm or Exact SDF geometry?
1.CMC33;     2.STL model;      3.Exact SDF geometry.
You can choose by entering the numbers 1, 2 and 3, where 1 and 2 correspond to the implementations of Algorithm 1 
and Algorithm 2 in the article, respectively, and 3 is some additional standard geometry provided, for which we have 
accurately reconstructed the level set and the flow field; subsequently, you can choose the test case, where the 
initial flow field will be subjected to a constrained optimisation algorithm for obtaining a high-quality uniform 
particle distribution. The resolution of the flow field can be self-defined as needed, this feature will be open in 
the nearest future. If you have any specific need, or discover any problem or bug, please leave a message and we will 
reply as soon as possible!

## Get Help

You can also view questions
and ask your own on our [GitHub Discussions]([https://github.com/AMReX-Codes/amrex/discussions](https://github.com/amrPX-Projects/amrPX-design.git)) page.
To obtain additional help, simply post an issue.

## Copyright Notice

Copyright (c) 2024, All rights reserved.

If you have any questions about your rights to use or distribute this tool, please contact the author.

## License

License for amrPX-design can be found at [LICENSE](LICENSE).

## Citation



