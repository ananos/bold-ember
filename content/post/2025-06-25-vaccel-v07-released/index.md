---
title: "vAccel v0.7 Released!"
date: 2025-06-25
draft: false
tags: ['news']
---

Simplified Session Management, Extended RPC Support, and Robust Backend Integration

<figure>
        <img src="/images/vaccel-logo.png#floatright" width="250px" alt="" />
</figure>

#### Key Features and Improvements

###### v0.7.0 Highlights  
*Released: [June 18, 2025](https://github.com/nubificus/vaccel/releases/tag/v0.7.0)*

- Enable runtime plugin loading and coexistence of remote and local plugins
- Allow selection of inference model at runtime
- Add unified config and enable explicit bootstrap/cleanup
- Refactor vAccel resources
- Enable robust plugin versioning and compatibility checks
- Cleanup and reorganize headers and plugin functions

###### v0.7.1 Highlights  
*Released: [June 24, 2025](https://github.com/nubificus/vaccel/releases/tag/v0.7.1)*

- Bug Fixes & Stability, Resolves memory issues and plugin initialization bugs.

##### Extending the vAccel Ecosystem

With its refactored resource architecture and plugin lifecycle improvements,
vAccel can now better support heterogeneous accelerators, serverless runtimes,
and secure offloading at the edge. These improvements build on ongoing research
into cloud-native compute offloading.

##### Availability

Source code and binaries are available under the Apache 2.0 License:

- [v0.7.0 Release Notes](https://github.com/nubificus/vaccel/releases/tag/v0.7.0)
- [v0.7.1 Release Notes](https://github.com/nubificus/vaccel/releases/tag/v0.7.1)

Visit the GitHub repository: [github.com/nubificus/vaccel](https://github.com/nubificus/vaccel)

##### About vAccel

vAccel is an open-source virtualization acceleration framework by Nubificus
LTD, enabling efficient offloading of compute workloads to accelerators or
remote endpoints across the edge–cloud continuum. It features modular plugins
for backends, transports, and runtimes, and is designed to work seamlessly with
containerized and serverless environments.

##### Hands-on! 

For more information, tutorials, and links, visit:
[https://docs.vaccel.org](https://docs.vaccel.org)

Contact:

- vaccel@nubificus.co.uk
- GitHub: [github.com/nubificus/vaccel](https://github.com/nubificus/vaccel)