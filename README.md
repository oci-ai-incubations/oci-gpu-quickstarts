# Oracle Cloud Infrastructure (OCI) GPU Onboarding Content
This repository hosts onboarding content for Oracle Cloud Infrastructure GPU offerings. It is organized by GPU family, with each folder providing:

1. A snapshot of each GPU hardware configuration 
2. A quick-start guide to provision GPU resources on OCI
3. A “Hello World” sample to verify compute and driver/toolchain readiness
4. Links to approved OS images and drivers
5. Guidance for running on Oracle Kubernetes Engine (OKE)
6. Basic and advanced health and issue diagnosis tools
7. A link to blogs and partner content covering advanced configurations, specifications


## Repository Structure

```
/nvidia
    /B200
        README.MD
    /GB200
        README.MD
    /xxx
        README.MD
/amd
    /MI300X
        README.MD
    /MI355X
        README.MD
```
Helper scripts for driver checks, GPU validation, and log collection
You can add additional GPU families as OCI expands offerings.

### Questions
Reach out to oci-gpu-quickstart-help@oracle.com 

## Contributing

This project welcomes contributions from the community. Before submitting a pull request, please [review our contribution guide](./CONTRIBUTING.md)

## Security

Please consult the [security guide](./SECURITY.md) for our responsible security vulnerability disclosure process

## License

Copyright (c) 2024 Oracle and/or its affiliates.

Released under the Universal Permissive License v1.0 as shown at
<https://oss.oracle.com/licenses/upl/>.
