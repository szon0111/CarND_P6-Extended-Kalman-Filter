# Project 6: Extended Kalman Filter
[//]: # (Image References)

[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)


Overview
---
Utilize a kalman filter to estimate the state of a moving object of interest with noisy lidar and radar measurements.

#### The goals / steps of this project are the following:
* Initialize Kalman filter variables
* Predict where our object is going to be after a time step Δt
* Update where our object is based on sensor measurements
* Make the prediction and update steps repeat themselves in a loop.
* Calculate root mean squared error comparing the Kalman filter results with the provided ground truth.
* Achieve RMSE <= [.11, .11, 0.52, 0.52] 

Project Deliverables
---
* `FusionEKF.cpp` initializes the filter, calls the predict function, calls the update function
* `kalman_filter.cpp` defines the predict function, the update function for lidar, and the update function for radar
* `tools.cpp` function to calculate RMSE and the Jacobian matrix

Results
---
**Dataset 1:**
X: 0.0964
Y: 0.0853
Vx: 0.4154
Vy: 0.4316

**Dataset 2:**
X: 0.0726
Y: 0.0965
Vx: 0.4216
Vy: 0.4932

---

## Dependencies

* Udacity Simulator [download](https://github.com/udacity/self-driving-car-sim/releases)
* uWebSocket [download](https://github.com/uWebSockets/uWebSockets)
* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)
