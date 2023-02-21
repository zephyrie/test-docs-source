########################
Toolkit Navigation
########################

*******************
Module Overview
*******************

We recommend going sequentially through each chapter and focusing on the specific types of tasks that you’re interested in (e.g., Radiology, Pathology, or Computer-Assisted Intervention).

For additional information on setting up your environment and using the MONAI Toolkit, check out **Chapter 1: Getting Started**.

If you are at the start of your journey and looking to understand how to speed up your image annotation process, check out **Chapter 2: Using MONAI Label**.

If you already have an annotated dataset and want to get started training with MONAI or integrate MONAI into your existing PyTorch Training Loop, take a **Chapter 3: Using MONAI Core**.

If you are interested in MONAI and Federated Learning working together, look at **Chapter 4: MONAI Federated Learning**.

If you are interested in some advanced topics and looking to compare benchmarks, interested in performance profiling, or looking for some researcher best practices with MONAI, check out **Chapter 5: Performance and Benchmarking**.

*****************************
Module 1. Getting Started
*****************************
Getting started with the MONAI Toolkit walks you through the various options you have when launching the Toolkit Container.

* Overview of MONAI Toolkit
* Installation Prerequisites
* Running the MONAI Toolkit - Jupyter Lab
* Running the MONAI Toolkit - Interactive Bash
* Changing Shared Memory Segment Size
* Access Jupyter Lab Remotely
* Mount Custom Data Directory

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
MONAI Core is the flagship library of Project MONAI that provides domain-specific capabilities for training AI models for healthcare imaging. It gives developers and researchers a PyTorch-driven library for deep learning tasks that includes everything they need to develop medical imaging training workflows.

MONAI Toolkit contains tutorials that will guide you through the various functions of MONAI Core, starting from the basics of I/O, Transforms, and Datasets. Then you'll learn more about complex tasks like Self-Supervised Learning and Auto3DSeg, and you'll find a gallery of tutorials covering technical topics like 3D segmentation, detection, registration, and reconstruction.

* Getting Started with MONAI-Core
* Customize Bundle Models and Datasets
* Auto3DSeg
* Self-Supervised Learning (SSL)
* Other MONAI-Core Application
   * Radiology
   * Pathology
   * Computer-Assited Intervention (CAI)

************************************
Module 4. MONAI Federated Learning
************************************
MONAI includes the federated learning (FL) client algorithm APIs that are exposed as an abstract base class for defining an algorithm to be run on any FL platform. NVIDIA FLARE, the FL platform developed by NVIDIA, has already built the integration piece with these new APIs.

MONAI Toolkit contains tutorials that guide you through getting started with MONAI Federated Learning and uses the FLARE FL Simulator to help researchers accelerate the development of federated learning workflows. It then discusses what a Real-world Federated Learning Deployment would look like and provides examples of how one would set up experiments in a real-world deployment.

* Getting started with MONAI Federated Learning (FL)
* MONAI FL in the Real World

*****************************************
Chapter 5. Performance and Benchmarking
*****************************************
Model training is often time-consuming in deep learning development, especially in medical imaging applications. Even with powerful hardware, workflows often require analysis and tuning for high performance. And using carefully chosen algorithms—such as network architectures, loss functions, and optimizers—can speed up training.

MONAI Toolkit contains details on performance benchmarking of MONAI Label and MONAI Core. It provides deep learning model training best practices for medical imaging that can improve performance in terms of efficiency and effectiveness and demonstrates how to analyze training pipelines, profile training pipelines, algorithms selection, and methods to optimize GPU utilization.
    
* MONAI Label Benchmarking
* MONAI Core Training
* Performance Optimization