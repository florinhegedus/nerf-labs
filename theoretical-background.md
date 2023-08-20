---
layout: default
title: Theoretical Background
description: Explore the core principles and mathematical foundations behind NeRFs
---

# Key Concepts

## Fields 
In physics, a field is a physical quantity that is associated with every point in space and time. It is a way of describing how a particular property or force is distributed throughout space. We can represent a field as a function mapping a coordinate x to a quantity, which is typically a scalar or vector. In practice, the underlying field generation process may not have a known analytic form. Thus, functions may be described by parameters that are hand crafted, optimized, or learned. Furthermore, we often index sampled functions using discrete values, such as at camera pixels, or choose discrete function parameterizations using voxels or discretized level sets.

## Radiance 
In physics, radiance is the measure of the quantity of light that passes through or is emitted from a particular area, and falls within a given solid angle. It measures the brightness of light that comes from a specific direction.

## Neural Networks
A neural network connects many layers of artificial neurons to learn to non-linearly map a fixed-size input to a fixed-size output. A multi-layer perceptron (MLP) neural network can approximate any function
through their learned parameters (universal approximation
theorem).

## Neural Fields 
Following the universal approximation theorem, any field can be parameterized by an MLP neural network. Thus, a neural field is a field that is parameterized fully or in part by a neural network. Neural fields are both continuous and adaptive by construction. Unlike the memory required for discrete parameterizations that scales poorly with spatio-temporal resolution, the memory required for neural fields instead scales with the number of parameters of the neural network—so-called network complexity.

## Neural Radiance Fields. 
A Neural Radiance Field (NeRF) is a fully-connected neural network that can generate novel views of complex 3D scenes, based on a partial set of 2D images. The NeRF model takes the 3D coordinates of points in space and the view direction as input and outputs the volume density and color at that point. The density indicates how much light is blocked by the point, while the color denotes the emitted radiance.

# Taxonomy
Categorizing NeRFs
