## UNDER CONSTRUCTION
**THIS PAGE IS UNDER CONSTRUCTION** 

# OCI GPU Quick Start: NVIDIA GB200
This document provides hardware specifications, supported OS images, onboarding verification, sample benchmarks, and best-practices for OCI deployments using the NVIDIA GB200 GPU shape.

# Table of Contents
* [Hardware Specifications](#hardware-specifications)
* [Recommended Operating Systems](#recommended-operating-systems)
    * [Recommended Software Version](#recommended-software-version)
    * [Custom OS Image Creation with Packer](#custom-os-image-creation-with-packer)
    * [Provided Images](#provided-images)
    * [Hello World Verification](#hello-world-verification)
* [Performance Benchmarks](#performance-benchmarks)
    * [NCCL](#nccl)
    * [Model Inference Performance](#model-inference-performance)
* [OKE GPU Getting Started](#oke-gpu-getting-started)
* [Troubleshooting](#Troubleshooting)
* [Further Reading & Support](#further-reading--support)

# Hardware Specifications

| Shape Name        | GPU Model     | GPUs/Node | GPU Memory | GPU Memory Total |             CPU           | # of CPUs | System Memory | Local Storage	 | Host NIC | RDMA (ROCe) NICs |
|-------------------|---------------|-----------|------------|----------------- |---------------------------|-----------|---------------|----------------|----------|-----------|
| <!-- Shape Name -->        |  <!-- GPU Model -->     |  <!-- GPUs/Node --> | <!-- GPU Memory -->  | <!-- GPU Memory Total --> |             <!-- CPU -->          | <!-- # of CPUs --> | <!-- System Memory --> | <!-- Local Storage -->	 | <!-- Host NIC --> | <!-- RDMA (ROCe) NICs --> |

*See the [OCI Compute Shapes Docs](https://docs.oracle.com/en-us/iaas/Content/Compute/References/computeshapes.htm) for up-to-date details.

# Recommended Operating Systems

## Recommended Software Version

## Custom OS image Creation with Packer

To build your images using packer clone the OCI HPC Images repo and run the commands found there [OCI HPC Images GitHub Repo](https://github.com/oracle-quickstart/oci-hpc-images/blob/main/README.md).

## Provided Images

| OS Version        | Image Packer Build Details       | OCI Platform Image Link                                                                        | Driver Versions | Build & Dependency Status | 
|-------------------|-------------------------------|------------------------------------------------------------------------------------------------------------|--------------|--------------------------|

## Hello World Verification

# Performance Benchmarks

## NCCL 

## Model Inference Performance

# OKE GPU Getting Started

# Troubleshooting

Here you can find suggested troubleshooting methods.

# Further Reading & Support
1. Blog on GB200 hardware & its multi node performance AI for Employees

