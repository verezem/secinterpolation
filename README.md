# secinterpolation
This is the python program which aims to simplify the correct interpolation of spatially inhomogeneous oceanographic section data on the regular grid of numerical model (the presented case is NEMO grid). The proposed tool uses the Gaussian core interpolation method where core size and thus to-be-interpolated points weights are defined according to their number and distance from the target regular grid point. 
Gaussian weights are defined as: 
weight = exp(-kx*x_dist^2 - ky*y_dist^2), 
where kx = 10^3/STD(x_dist)^2 and ky = 10^4/STD(y_dist)^2
