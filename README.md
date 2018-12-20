Flip-Angle-Design-Toolbox
=========================

Tools for designing optimal flip angle schemes for hyperpolarized carbon-13 magnetic resonance spectroscopy. 

The Flip Angle Design Toolbox provides a framework for specifying a linear differential equation model 

dx/dt = A x(t) + B u(t) 

to describe magnetization dynamics and tools for maximum likelihood and least-squares estimation of unknown model parameters. Toolbox also provides routines to generate optimal flip angle schemes for design objectives including: 
* maximizing signal-to-noise ratio 
* and providing minimum-variance estimates of model parameters. 

The MATLAB script DEMO.m provides a demonstration of the toolbox's capabilities. The main functionalities are:
* a class linear_exchange_model for specifying a model of the magnetization dynamics 
* a function generate_data for computing simulated observation trajectories generated by the model 
* a function optimal_flip_angle_design for computing optimal flip angle schemes 
* a function parameter_estimation for computing maximum likelihood or least-squares estimates of unknown model parameters. 

This toolbox requires that the following MATLAB toolboxes are installed:
* Optimization Toolbox
* Symbolic Math Toolbox 

Technique described in:
* https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5134417/
* https://dx.doi.org/10.1109%2FTMI.2016.2574240
