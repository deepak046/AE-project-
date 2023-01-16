# Applied Estimation Project

### Authors: Deepak Ganesh, Tawsiful Islam, Magnus Tibbe


Here is the [Project Report](https://github.com/deepak046/AE_project/blob/main/AE_project_report.pdf) 

We have also made a [movie](AE_project/Double_Pendulum_movie.mp4) that shows how the position is begin estimated for a Double Pendulum by both EKF and UKF

## How our code works:

[State transition function](AE_project/state_trans.m) is a MATLAB function that contains the implementation for propagation of the states (angles) through time.
    returns - all the propagated states through the entirety of the simulation

[Extended Kalman Filter function](AE_project/EKF.m) is a MATLAB function that contains the implementation of EKF state estimation for both simple and double pendulum by calculating their jacobians.
    returns - Estimated state, Estimated Covariance for current state

[Unscented Kalman Filter function](AE_project/UKF.m) is a MATLAB function that contains the implementation of UKF state estimation for both the systems
    returns - Estimated state, Estimated Covariance for current state

[Simple Pendulum](AE_project/Simple_Pendulum.m) - main MATLAB script that contains the implementation for Simple Pendulum by gathering information from state_trans, EKF and UKF functions, and plotting the graphs of simulation, errors and the covariance values over time.

[Double Pendulum](AE_project/Double_Pendulum.m) - main MATLAB script that contains the implementation for Double Pendulum


## Instructions:

Run the [Simple Pendulum](AE_project/Simple_Pendulum.m) (or) [Double Pendulum](AE_project/Double_Pendulum.m) script directly to see results for that respective system. 
    - The first part of the script has parameter values such as Q, R and initial angles that
    can be tweaked to test the simulations.
 
