# Heat Transfer Projects

## English

This repository contains a simulation project in Thermodynamics, more specifically, in Heat Transfer, which was originally started as part of the Heat Transfer course at Universidad de los Andes, but has been significantly extended by the author to make them significantly more comprehensive and more fully fledged as simulation programs.



### **Automated design of a fin**

This project consists of a simulation of the heat profile and efficiency of a heat dissipating fin, which has some given geometric constraints. The program uses a gradient descent method as a means to maximize fin efficiency and then plots the evolution of this optimization process.

This project should receive user defined values for the physical parameters, but as of now these are hard-coded (but can be easily changed in code without affecting the model). The [optimization evolution](Project1_FinOptimization/optimization_evolution.png) file only presents a few initial iterations of optimization, as the program has not been run completely since the recent correction of a series of bugs coming from the original version.

The program utilizes a computationally intensive method for surface area calculation which affects performance significantly; nonetheless, this method has been left in the code as it has been the only attempted strategy which provides consistently accurate results. This aspect will be re-evaluated in future versions. A bug that allows for impossible temperature profiles is present, but is only effectful with some fin profiles that possess sharp changes in cross-section. This will be fixed in a future version. An adiabatic boundary condition at the fin tip is used; changes will be made to allow for different boundary conditions to be applied. Some further changes will be made regarding the program's graphical outputs.

The interactive version, as of now, serves as a debugging environment only and is not used to actually perform simulation work.

*A document with the mathematical formulation of the discretizations used (these are not trivial) will be uploaded soon.*
