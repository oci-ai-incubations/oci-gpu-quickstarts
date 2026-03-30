> [!WARNING]
> **INTERNAL USE ONLY — NOT FOR PUBLIC DISTRIBUTION**
> This document has not been approved for public release. It must not be committed to a public repository or shared externally until this notice is explicitly removed by the document owner prior to merge.

# OCI GPU Quick Start: <Vendor> <GPU_FAMILY>

This document provides hardware specifications, supported OS images, onboarding verification, sample benchmarks, and best-practices for OCI deployments using the <Vendor> <GPU_FAMILY> GPU shape.

## At a Glance

- Shape: `<shape name>`
- GPU configuration: `<gpu model and count>`
- Recommended OS baseline: `<minimum supported OS>`
- Recommended software baseline: `<primary driver/CUDA or ROCm/NCCL or RCCL>`
- Primary verification command: `<hello world or device visibility command>`
- Operational profile: `<single-node, scale-out, topology-sensitive, etc.>`

# Table of Contents
* [Hardware Specifications](#hardware-specifications)
* [Recommended Operating Systems](#recommended-operating-systems)
    * [Recommended Software Version](#recommended-software-version)
    * [Custom OS Image Creation with Packer](#custom-os-image-creation-with-packer)
    * [Provided Images](#provided-images)
    * [Hello World Verification](#hello-world-verification)
* [Performance Benchmarks](#performance-benchmarks)
* [OKE GPU Getting Started](#oke-gpu-getting-started)
* [Troubleshooting](#troubleshooting)
* [Further Reading & Support](#further-reading--support)

# Hardware Specifications

| Shape Name | GPU Model | GPUs/Node | GPU Memory (GB/GPU) | GPU Memory Total | CPU | # of CPUs | System Memory | Local Storage | Host NIC | RDMA (ROCe) NICs |
|---|---|---|---|---|---|---|---|---|---|---|
| <!-- Shape Name --> | <!-- GPU Model --> | <!-- GPUs/Node --> | <!-- GPU Memory --> | <!-- GPU Memory Total --> | <!-- CPU --> | <!-- # of CPUs --> | <!-- System Memory --> | <!-- Local Storage --> | <!-- Host NIC --> | <!-- RDMA (ROCe) NICs --> |

See the [OCI Compute Shapes Docs](https://docs.oracle.com/en-us/iaas/Content/Compute/References/computeshapes.htm) for up-to-date details.

# Recommended Operating Systems

## Recommended Software Version

## Custom OS Image Creation with Packer

To build your images using packer clone the OCI HPC Images repo and run the commands found there [OCI HPC Images GitHub Repo](https://github.com/oracle-quickstart/oci-hpc-images/blob/main/README.md).

## Provided Images

| OS Version | Image Packer Build Details | OCI Platform Image Link | Driver Versions | Build & Dependency Status |
|---|---|---|---|---|

## Hello World Verification

# Performance Benchmarks

# OKE GPU Getting Started

# Troubleshooting

Here you can find suggested troubleshooting methods.

# Further Reading & Support
