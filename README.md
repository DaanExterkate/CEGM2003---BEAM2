# CEGM2003---BEAM2
This project is made by master students of the TU Delft for the Course CEGM2003. 

The project uses Physics Informed Neural Networks (PINN's) to simulate dynamic beam behaviour. It consists of two parst, both parts have a separate fully self-explanatory notebook:

1. Euler-Bernoulli Beam.
This first notebook simulates beam behaviour of a Euler-Bernoulli beam. Section 1.1 solves the Euler-Bernoulil problem. A PINN has been build and trained to predict the bending u given boundary and initial conditions. In section 1.2 the predicted solution of u is plotted against the time with a high testing accuracy. Finally, in section 1.3, we take the velocity, acceleration and bending moment from the predicted values of u by the PINN and compare them with their analytical solution.  

2. Timoshenko Beam.
This second notebook simulates beam behaviour of the Timoshenko beam. Two problems are distinguished, explained in separate sections. Section 2.1 solves the so-called Timoshenko forward problem. In this problem a PINN is build predicting $\theta$ and w given boundary and initial conditions. Section 2.2 deals with the Timoshenko Inverse problem. In this problem a PINN is build predicting the force function g(x,t) alongside $\theta$ and w given observations of $\theta$ and w.

To execute the code, clone or download the notebooks and run them, preverably on a GPU. For more information about the benefits of PINN, see below.

Enjoy reading. For information 

By group BEAM 2:
Jur Bokkers, Hidde Drost, Bastiaan Kurstjens, Amco de Jong and Daan Exterkate. 


## Why are we using PINNs? 

Todays engineering challenges involve addressing the connection of subsystems and managing uncertainties in behavior resulting from both internal and external variables and their interactions. Furthermore, the prediction of for example engineering structures are challenging because of their overall complex behaviour. Such complex engineering system behaviour can be described by PDE's. We can use these PDE's to understand their behaviour. Examples of such physical problems are; catenary-pantograph interactions in railways, simulating air turbulence that disrupts flights and in our case; structural beam's behavior. In practice, the used equations are too complicated to solve analytically and finite element modelling has also some complications when structures become too big. 

PINNs combine knowledge on the underlying physical theory (PDEs) and the knowledge on deep learning. PINNs are potentially more efficient since, once trained, the investigated are much faster known than for example in finite element modelling. 

For this excercise, structural behaviour of a beam is investigated considering the Euler Bernoulli beam theory as well as the Timoshenko beam theory. Important note to make here; this is a very specific problem from which PDEs can be solved analytically. In addition, the forcing is approximated with a sine and cosine function. However, in real-life this is not case. External forcing of for example a bridge can not be described by such an sinisoidal function, neither can a solution to the PDE be found analytically. However, this excercise shows the potential of PINNs since it is able to predict exact behavior very precisely.
