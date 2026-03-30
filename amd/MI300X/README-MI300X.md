# UNDER CONSTRUCTION
**THIS DOCUMENT IS UNDER CONSTRUCTION**

# OCI GPU Quick Start: AMD MI300X Instinct GPU
This document provides hardware specifications, supported OS images, onboarding verification, sample benchmarks, and best-practices for OCI deployments using the AMD MI300X GPU bare-metal shape.

**Docs & technical content coming soon**

## At a Glance

- Shape family: `MI300X`
- Status: `under construction`
- Intended workload profile: `large-scale AI/ML and HPC`
- Primary verification flow: `to be updated`

# Table of Contents
* [Hardware Specifications](hardware-specifications)
* [Recommended Operating Systems](#recommended-operating-systems)
    * [Recommended Software Version](#recommended-software-version)
    * [Custom OS Image Creation with Packer](custom-os-image-creation-with-packer)
    * [Provided Images](provided-images)
* [Hello World Verification](hello-world-verification)
* [Performance Benchmarks](performance-benchmarks)
    * [RCCL & Model Inference Performance](rccl--model-inference-performance)
* [OKE GPU Getting Started](oke-gpu-getting-started)
* [Troubleshooting](Troubleshooting)
* [Further Reading & Support](further-reading--support)

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

# Hello World Verification

# Performance Benchmarks

## RCCL & Model Inference Performance

# OKE GPU Getting Started

# Troubleshooting

Here you can find suggested troubleshooting methods.

## Further Reading & Support

### AMD Technical Documents
1. [AMD ROCM Software Compatibility Matrix](https://rocm.docs.amd.com/en/latest/compatibility/compatibility-matrix.html1)
2. [AMD ROcm Software Examples](https://github.com/ROCm/rocm-examples)
3. [AMD Kubernetes GPU Operator](https://github.com/ROCm/gpu-operator)

### OCI AMD 300X Technical Docs & Supported Solutions

1. [OCI GPU Scanner - Cluster Health Management Solution](https://github.com/oracle-quickstart/oci-gpu-scanner)
2. [OCI HPC SLURM Deployed Terraform Stack](https://github.com/oracle-quickstart/oci-hpc)
3. [OCI HPC OKE Deployment Stack](https://github.com/oracle-quickstart/oci-hpc-oke)
