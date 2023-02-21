######################
System Requirements
######################

****************************
Installation Prerequisites
****************************

Using the `MONAI Toolkit Container <https://catalog.ngc.nvidia.com/orgs/nvidia/teams/clara/containers/monai-toolkit>`__ requires the host system to have the following installed:

*  `Docker Engine <https://docs.docker.com/get-docker/>`__
*  `NVIDIA GPU Drivers <https://docs.nvidia.com/datacenter/tesla/tesla-installation-notes/index.html>`__
*  `NVIDIA Container Toolkit <https://github.com/NVIDIA/nvidia-docker>`__

The MONAI Toolkit 1.0 is based on the `NVIDIA PyTorch container <https://catalog.ngc.nvidia.com/orgs/nvidia/containers/pytorch>`__ release 22.09. The embedded CUDA 11.8.0 requires NVIDIA Driver release 520 or later. However, if you are running on a data center GPU (for example, T4 or any other data center GPU), you can use NVIDIA driver release 450.51 (or later R450), 470.57 (or later R470), 510.47 (or later R510), or 515.65 (or later R515). 

The CUDA driver's compatibility package only supports particular drivers. Thus, users should upgrade from all R418, R440, and R460 drivers, which are not forward-compatible with CUDA 11.8

No other installation, compilation, or dependency management is required. It is not necessary to install the NVIDIA CUDA Toolkit.

For a full list of supported software and specific versions that come packaged with the frameworks based on the container image, see the `Framework Containers Support Matrix <https://docs.nvidia.com/deeplearning/frameworks/support-matrix/index.html>`__ and the `NVIDIA Container Toolkit Documentation <https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html>`__.


****************************
Hardware Requirements
****************************

MONAI Toolkit has been validated on V100 and A100 GPUs, but should generally be supported on GPUs such as H100, A100, A40, A30, A10, V100, and more.

The following system configuration is recommended to achieve reasonable training and inference performance with MONAI Toolkit and supported models provided.

*  At least 12GB of GPU RAM and up to 32GB depending on the network or model you use
*  At least 32 GB of RAM - and the more RAM the better
*  At least 50 GB of SSD Disk Space

For a complete list of supported hardware, please see the `NVIDIA AI Enterprise Product Support Matrix <https://docs.nvidia.com/ai-enterprise/latest/>`__