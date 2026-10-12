# Autonomous-Vehicle---ECE148


An autonomous vehicle project for **ECE/MAE 148: Introduction to Autonomous Vehicles** at UC San Diego.

This project will use **DonkeyCar**, **DonkeySim**, Python, Linux, and machine learning to develop and test an autonomous driving system before applying concepts to a physical robotic vehicle.

The goal is to build a vehicle capable of learning from human driving data, navigating a track autonomously, and eventually integrating the trained autonomy stack with a physical RC vehicle.

---

## Project Goals

The project is planned around the following objectives:

- Collect driving data using DonkeyCar and DonkeySim
- Train a neural network using behavioral cloning
- Allow the trained model to predict steering and throttle from camera images
- Improve autonomous lap consistency and speed
- Test the vehicle on the Warren track in DonkeySim
- Evaluate models using lap time and autonomous driving reliability
- Experiment with different throttle limits and steering behavior
- Test autonomous models on a remote simulation server
- Apply lessons learned in simulation to a physical autonomous vehicle
- Explore integration with ROS 2 and robotics software

---

## Simulation Environment

The first stage of the project uses **DonkeySim** with the DonkeyCar framework.

The vehicle is being developed and tested on the:

**Warren Track**

The simulated vehicle receives camera frames and uses a trained neural network to predict:

- Steering angle
- Throttle

Human driving data is recorded as image, steering, and throttle samples and later used to train the autonomous driving model.

### Planned Workflow

```text
Human Driving
      ↓
Camera Images + Steering + Throttle
      ↓
Training Dataset
      ↓
Behavioral Cloning Neural Network
      ↓
Predicted Steering + Throttle
      ↓
Autonomous Vehicle