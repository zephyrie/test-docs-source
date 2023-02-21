###################
Toolkit Libraries
###################

********************
Software Versions
********************

=========== =======
Software    Version
=========== =======
MONAI Core  1.0.1
MONAI Label 0.5.2
NVFlare     2.2.1
=========== =======

*************
MONAI Label
*************

MONAI Label minimizes the need for developers and researchers to manually annotate data by providing an intelligent imaging labeling and learning SDK that can be integrated into either customized or template-based data labeling apps. MONAI Label saves developers time, helping them quickly progress to training, tuning, and validating their medical AI models within the MONAI standardized paradigm.

The industry’s most popular open source viewers already have MONAI integrated: 3D Slicer, OHIF, QuPath, Digital Slide Archive, and CVAT, and it is also integrated into cloud service providers. Developers can also incorporate MONAI Label into their custom viewer using server and client APIs, which are well abstracted and documented for seamless
integration.

MONAI Label has enhanced active learning capabilities, which is a process that aims to use the least amount of data to achieve the highest possible model performance. Choosing data that will have the most significant influence on your overall model accuracy allows human annotators to focus on the annotations that will have the highest impact on the model performance. Developers can see up to a 75% reduction in training costs with active learning in MONAI Label with increased labeling and training efficiency while achieving better model performance.

`MONAI Label Developer Page <https://monai.io/label.html>`__

************
MONAI Core
************

MONAI Core gives developers and researchers a PyTorch-driven library for deep learning tasks that includes domain-optimized capabilities they need for developing medical imaging training workflows. Performance features such as MONAI Core’s AutoML, Smart Caching, GPU-accelerated I/O, and transforms take training from days to hours, and hours to
minutes, helping users accelerate AI into clinical production.

With Auto3D segmentation, developers can train models with 1-5 lines of code that can quickly segment regions of interest in data from 3D imaging modalities like CT and MRI, reducing training time from weeks/months to 2 days. And MONAI Core’s federated learning client algorithm APIs are exposed as an abstract base class for defining an
algorithm to run on any federated learning platform. NVIDIA FLARE has already built the integration piece with these new APIs. And using MONAI Bundle configurations with the new federated learning APIs means developers can take any bundle and seamlessly extend them to a federated paradigm.

`MONAI Core Developer Page <https://monai.io/core.html>`__

**************
NVIDIA FLARE
**************

NVIDIA FLARE (NVIDIA Federated Learning Application Runtime Environment) is a domain-agnostic, open-source, extensible SDK that allows researchers and data scientists to adapt existing ML/DL workflows (PyTorch, RAPIDS, Nemo, TensorFlow) to a federated paradigm. It enables platform developers to build a secure, privacy-preserving offering for a
distributed multi-party collaboration. Built on a componentized architecture, NVIDIA FLARE gives you the flexibility to take federated learning workloads from research and simulation to real-world production deployment.

MONAI includes the federated learning client algorithm APIs exposed as an abstract base class for defining an algorithm to run on any federated learning platform. NVIDIA FLARE has already built the integration piece with these new APIs.

`NVIDIA FLARE Developer Page <https://developer.nvidia.com/flare>`__