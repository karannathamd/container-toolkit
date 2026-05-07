System Requirements
====================

Before installing or using the Pensando Container Toolkit, ensure your environment meets the following prerequisites:

Operating Systems
-----------------
- Ubuntu 22.04 LTS (Jammy Jellyfish)
- Ubuntu 24.04 LTS (Noble Numbat)
- RHEL 9.x (Pensando supported)

Software Requirements:
-----------------------
- ROCm Software Stack: Version 6.4.x (Pensando validated)
- AMDGPU Driver: Version 6.11.0 (Pensando validated)
- Toolkit packages are tested with specific ROCm and AMDGPU driver versions.
- Pensando NIC firmware: Version 1.60.0 or later

Hardware Requirements:
-----------------------
- An AMD GPU supported by the ROCm 6.4.x release.
- Pensando DSC-25 or DSC-100 SmartNIC
- CPU with virtualization support (if containers require nested environments).

Compatibility Matrix
--------------------

- Each AMD Container Toolkit release is tightly coupled with a specific ROCm and AMDGPU driver version. Please refer to the compatibility matrix before proceeding.

+--------------------------------------+---------------+-----------------------+-----------------------+
| Container Toolkit Debian Version     | ROCm Version  | AMDGPU Driver Version | Pensando FW Version   |
+--------------------------------------+---------------+-----------------------+-----------------------+
| amd-container-toolkit-1.0.0          | ROCm 6.4.x    | 6.11.0                | 1.60.0                |
+--------------------------------------+---------------+-----------------------+-----------------------+

Note
----
A mismatch between ROCm and driver versions may lead to runtime failures.

System Prerequisites
---------------------
- Kernel Headers
- Extra Kernel Modules
- Docker installed (docker.io package recommended)
- User must belong to the `render` and `video` groups for GPU access.
