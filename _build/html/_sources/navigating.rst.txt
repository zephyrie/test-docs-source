########################
Toolkit Navigation
########################

*******************
Module Overview
*******************

To get the most out of the MONAI Toolkit, we recommend going through each module sequentially and focusing on the specific tasks that interest you. The following chapters provide a comprehensive guide to using MONAI:

- **Module 1: Getting Started** - This module provides information on setting up your environment and using the MONAI Toolkit.
- **Module 2: Using MONAI Label** - If you’re at the start of your journey and want to learn how to speed up your image annotation process, check out this module.
- **Module 3: Using MONAI Core** - If you already have an annotated dataset and want to get started training with MONAI or integrate MONAI into your existing PyTorch training loop, this module is for you.
- **Module 4: MONAI Federated Learning** - If you’re interested in MONAI and Federated Learning working together, check out this module.
- **Module 5: Performance and Benchmarking** - For advanced topics, including benchmarking, performance profiling, and researcher best practices with MONAI, take a look at this chapter.


*****************************
Module 1. Getting Started
*****************************
MONAI Label is an open-source platform for medical data labeling and learning. It offers advanced active learning strategies that enable users to create annotated datasets and develop AI annotation models for clinical evaluation. Sample apps covering various medical imaging modalities are provided, and the platform supports multiple viewer tools and datastore platforms.

Ready to start your journey with MONAI Label? Choose the modality that makes the most sense for your project and explore the sample apps provided. With the MONAI Toolkit, creating high-quality labeled datasets for medical AI applications has never been easier.

- MONAI Label for Radiology
- MONAI Label for Endoscopy
- MONAI Label for Pathology
- Bring your own Data
- Create your own Application
- Integration Guide

*****************************
Module 2. Using MONAI Label
*****************************
MONAI Label is an intelligent open-source image labeling and learning tool that enables users to create annotated datasets and build AI annotation models for clinical evaluation. 

MONAI Toolkit contains the MONAI Label and provides a plug-and-play environment for users. With a one-step setup of client viewers, MONAI Label allows researchers and developers to benefit from an interactive AI-Assisted labeling experience, including tutorials for different labeling scenarios.

* MONAI Label for Radiology
* MONAI Label for Endoscopy
* MONAI Label for Pathology
* Bring your own Data
* Create your own Application

*****************************
Module 3. Using MONAI Core
*****************************
MONAI Core is the flagship library of Project MONAI that provides domain-specific capabilities for training AI models for healthcare imaging. With PyTorch at its core, MONAI Core provides developers and researchers with a powerful toolkit for building deep learning models for medical image analysis.

Thanks to MONAI Core’s AutoML, Smart Caching, GPU accelerated I/O, and image transforms, users can train models faster than ever before, reducing training times from days to hours or even minutes. The library’s components facilitate deep learning in medical image analysis at various levels of granularity, while the APIs are designed to be lightweight, flexible, and easy to use. These building blocks can be easily integrated into existing PyTorch programs and larger systems, making it simple for users of all expertise levels to set up efficient and robust model training or evaluation pipelines for their healthcare imaging applications.

- Getting Started with MONAI Core
- MONAI Bundles and MONAI Models on NGC
- Auto3DSeg
- nnUNet
- Self-Supervised Learning (SSL)
- Experiment Management
- Lazy Resampling
- MetricsReloaded
- Tutorial Catalog
  - Radiology
  - Pathology
  - Computer-Assisted Intervention (CAI)

************************************
Module 4. MONAI Federated Learning
************************************
MONAI’s Federated Learning (FL) client algorithm APIs provide a robust and secure framework for collaborative medical image analysis. With these APIs, custom Federated Learning algorithms can be defined as an abstract base class and run on any Federated Learning platform.

NVIDIA FLARE, the Federated Learning platform developed by NVIDIA, has already integrated these APIs, making it easy to extend MONAI bundles to a federated paradigm and execute them using single- or multi-GPU training. Collaborative medical image analysis using MONAI’s FL enables healthcare providers and researchers to work together efficiently and effectively, without the need to share sensitive data. This approach facilitates the discovery of new insights and faster progress towards better patient outcomes.

- Getting started with MONAI Federated Learning
- MONAI Federated Learning with Local Provisioning
- NVIDIA Federated Learning Dashboard in the Cloud

*****************************************
Module 5. Performance and Benchmarking
*****************************************
Model training is often a time-consuming process in deep learning development, especially in medical imaging applications. Volumetric medical images are large in data size (e.g. multidimensional arrays) and the model training process can be complex. Even with powerful hardware (such as CPU/GPU with large RAM), workflows often require analysis and tuning for high performance. And using carefully chosen algorithms—such as network architectures, loss functions, and optimizers—can speed up training.

To provide an overview of performance benchmarking and improvement in practice, this chapter details basic metric numbers for MONAI Label and MONAI Core, how to analyze training pipelines, profile training pipelines, algorithms selection, and methods to optimize GPU utilization.

- MONAI Label Benchmarking
- MONAI Core Training
- Performance Optimization
- Multi-GPU Training
- Multi-Node Training
- TensorRT Conversion