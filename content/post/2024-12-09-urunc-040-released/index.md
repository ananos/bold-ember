---
title: "urunc 0.4.0 Released!"
date: 2024-12-09
draft: false
tags: ['news']
---

<figure>
        <img src="/images/urunc-logo.png#floatright" width="70px" alt="" />
        <img src="/images/docker-logo.webp#floatright" width="70px" alt="" />
</figure>

Nubificus proudly announces the release of `urunc` 0.4.0, the next-generation
unikernel container runtime. This release introduces new features, internal
improvements, and expanded documentation, reflecting our commitment to enabling
lightweight, secure, and high-performance unikernel adoption in modern
containerized environments.

#### What’s new in `urunc` 0.4.0?

##### New Features

- Docker Support: Seamless integration with Docker for broader compatibility
  and usability.
- Seccomp Support in VMMs: Enhanced security through syscall filtering.
- Block Image Support: Ability to use block images directly within `urunc`'s
  container image.
- Configurable Memory: Dynamically allocate memory based on container
  specifications.

##### Documentation Revamp

`urunc`'s documentation has undergone a significant overhaul, now providing
detailed guidance for users & developers. Explore the [new
documentation](https://nubificus.github.io/urunc).


##### Enhancements to Internals

- Network Cleanup: Automated deletion of TC rules and TAP devices when
  terminating unikernels.
- Advanced Unikernel Interface: New functions for checking supported features, such as:
  - `Init()`: Initializes the unikernel structure based on arguments.
  - `SupportsBlock()`: Verifies block device support.
  - `SupportsFS()`: Checks compatibility with specific filesystem types.
- Devmapper Enhancements: Refactored snapshot handling with a new
  `USE_DEVMAPPER_AS_BLOCK` environment variable.
- Static Networking: Enabled NAT and IP forwarding for improved connectivity.

##### Annotations

Urunc now supports custom annotations to streamline unikernel configurations:

- `com.urunc.unikernel.block`: Specifies the block image path within the
  container.
- `com.urunc.unikernel.blkMntPoint`: Defines the mount point for the block
  image.
- `com.urunc.unikernel.unikernelVersion`: Indicates the version of the
  unikernel.

##### CI/CD and Building Improvements

- New actions for unit testing and a restructured CI job workflow.
- Transition to Github ARC runners for enhanced efficiency.
- Build system refactor to improve usability and flexibility.


##### Miscellaneous Updates

- Support for Unikraft boot on arm64 Firecracker.
- Refactor of container handling and improvements in path and annotation management.
- Bug fixes and internal refinements to ensure stability and performance.

#### Why This Matters

`urunc` 0.4.0 represents a step forward in making unikernels a practical and
efficient choice for modern workloads. By introducing features like Docker
support and block image compatibility, it bridges the gap between traditional
containers and unikernels, offering a hybrid solution tailored to the needs of
today’s developers.

##### Quote from the Team

“This release is the result of tireless work and collaboration across our team.
With `urunc` 0.4.0, we are giving developers the opportunity to fully leverage
the advantages of unikernels without sacrificing usability or compatibility
with existing ecosystems”.

Explore `urunc` 0.4.0 today! Discover the [full release
details](https://github.com/nubificus/urunc/releases/tag/v0.4.0) and download
[`urunc` 0.4.0](https://github.com/nubificus/urunc/releases/tag/v0.4.0) from
GitHub.

Stay tuned for our next planned release featuring shared FS support, WASM
unikernel support, MirageOS and many more! 

##### About Urunc
<figure>
        <img src="/images/urunc-logo.png#floatleft" width="50px" alt="" />
</figure>
Urunc is an open-source unikernel container runtime, designed to unlock the
potential of unikernels in cloud-native environments. By combining efficiency,
security, and ease of use, Urunc sets a new standard for lightweight container
orchestration.