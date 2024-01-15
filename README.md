# CEGM2003---BEAM2
This project is made by master students of the TU Delft for the Course CEGM2003. 

The project uses Physics Informed Neural Networks (PINN's) to simulate dynamic beam behaviour. It consists of two parst, both parts have a separate fully self-explanatory notebook:

1. Euler-Bernoulli Beam.
In this first file .....

2. Timoshenko Beam.
This second notebook simulates beam behaviour of the Timoshenko beam. Two problems are distinguished, explained in a separate sections. Section 2.1 solves the so-called Timoshenko forward problem. In this problem a PINN is build predicting $\theta$ and w given boundary and initial conditions. Section 2.2 deals with the Timoshenko Inverse problem. In this problem a PINN is build predicting the force function g(x,t) alongside $\theta$ and w given observations of %\theta% and w.

To execute the code, clone or download the notebooks and run them, preverably on a GPU.
Enjoy reading.

By group BEAM 2:
Jur Bokkers, Hidde Drost, Bastiaan Kurstjens, Amco de Jong and Daan Exterkate. 
