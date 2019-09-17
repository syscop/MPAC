# Motion Planning And Control (MPAC)

This repository contains a collection of algorithms for Motion Planning And Control (MPAC).

___

## Installation

MPAC is developed on Julia 1.2, but it should run on any Julia 1.x.
Run `] add https://github.com/syscop/MPAC` to install it.

### Test your installation

`] test MPAC`
___

## Documentation

There is no central documentation (yet). A good starting point is the overview of the package contents below. Use `?` to get documentation on the individual functions and commands.

___

## Contents

*Note: This package is under development and the implementations will be added over time.*

### RRT

A quick and simple implementation of the RRT algorithm.

### Utils

Provides:

* Data type definitions
* Distance Function implementations
* Implementations of evaluation metrics

### Robots

Defines the abstract robot type and some specific robots that are derived from it:

* Linear: A type for robots with linear dynamics. Example: puck
* Linearized Robot: A type for nonlinear robots that are linearized for planning.

It includes the implementation of several functions for the individual types. For example:

* the dynamics `dynamics`

### Visualizer

A small wrapper for the MeshCat visualizer, that allows for the 3-D visualization of structures by Utils as detailed [above](#Utils).
