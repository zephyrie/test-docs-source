##################
Introduction
##################

****************
MONAI Overview
****************

NVIDIA co-founded Project `MONAI <https://monai.io/>`__, the Medical Open Network for AI, with the world’s leading academic medical centers to establish an inclusive community of AI researchers to develop and exchange best practices for AI in healthcare imaging across academia and enterprise researchers.

`MONAI <https://monai.io/>`__ is the domain-specific, open-source Medical AI framework that drives research breakthroughs and accelerates AI into clinical impact. MONAI unlocks the power of medical data to build deep learning models for medical AI workflows. MONAI provides the essential domain-specific tools from data labeling to model training, making it easy to develop, reproduce and standardize medical AI lifecycles.

******************
MONAI Enterprise
******************

**MONAI Enterprise** is NVIDIA’s offering for enterprise-grade use of MONAI with an `NVIDIA AI Enterprise (NVAIE) <https://www.nvidia.com/en-us/data-center/products/ai-enterprise/>`__ 3.0 license. MONAI Enterprise on NVAIE 3.0 offers the MONAI Toolkit container, which provides enterprise developers and researchers with a secure, scalable workflow to develop medical imaging AI.

.. list-table:: MONAI Open-Source versus MONAI Toolkit with NVIDIA AI Enterprise
   :widths: 70 15 10
   :header-rows: 1

   * - Features
     - MONAI Open-Source
     - NVIDIA AI Enterprise
   * - | **Accelerated Tools and High-throughput Workflows** 
     - X
     - X
   * - | **Community Forum Support**
       | Submit questions to the MONAI Issues GitHub for Community Support  
     - X
     - X
   * - | **Full-stack and Business-critical Support**
       | Enterprise-grade support for multiple deployment options: bare-metal, containerized, cloud, and more
     - 
     - X
   * - | **Access to NVIDIA Experts**
       | Guidance on configuration and performance, including access to NVIDIA engineers
     - 
     - X
   * - | **Enterprise Training Services**
       | Instructor-led workshops and self-paced training for developers, data scientists, and IT professionals
     - 
     - X
   * - | **Security Notifications**
       | Receive priority notifications of the latest security fixes and maintenance releases
     - 
     - X
   * - | **Support for other NVIDIA Software and SDKs**
       | NVIDIA AI Enterprise also covers support for many other NVIDIA products, including RAPIDS, TensorRT, and more
     - 
     - X
   

******************
MONAI Toolkit
******************

**MONAI Toolkit** is a development sandbox offered as part of MONAI Enterprise, an NVIDIA AI Enterprise-supported distribution of MONAI. It includes a base container and a curated library of 9 pre-trained models (CT, MR, Pathology, Endoscopy), available on `NGC <https://ngc.nvidia.com/>`__, that allows data scientists and clinical researchers to jumpstart AI development. The base container includes the following:

-  MONAI Label: An intelligent labeling and learning tool with active learning that reduces data labeling costs by 75%
-  MONAI Core: A training framework to build robust AI models with self-supervised learning, federated learning, and Auto3D segmentation.
  
   -  With federated learning, APIs algorithms built with NVIDIA FLARE, MONAI can run on any federated learning platform.
   -  Auto3DSeg is domain-specialized AutoML for 3D segmentation, accelerating the development of medical imaging models and maximizing researcher productivity and throughput. Developers can get started with 1-5 lines of code, reducing training time from weeks/months to 2 days.

-  MONAI Model Zoo: A curated library of 9 pre-trained models (CT, MR, Pathology, Endoscopy) that allows data scientists and clinical researchers to jumpstart AI development
-  Curated Jupyter notebooks and tutorial resources to ease the onboarding process.

***************************
Who is this toolkit for?
***************************

=============
Researcher
=============

A Deep Learning Researcher’s role is to build novel domain-specific models and techniques to drive AI-powered acceleration for workflows or products. MONAI allows researchers to utilize standard building blocks to focus on creating their state-of-the-art AI models.

===============
Data Scientist
===============

A Data Scientist is a user/consumer of a research pipeline. The data scientist’s role is to adapt existing state-of-the-art domain techniques for specific data and use cases. They’ll refine and fine-tune the data science pipeline to fit the clinical workflow/application needed. MONAI aims to be easily integrated into existing pipelines, whether you
already have a PyTorch workflow or you’re just getting started on your task.

=======================
Application Developer
=======================

A platform developer aims to build a platform and service leveraging MONAI components that may include: - A labeling or active learning platform using MONAI Label - A complete ML platform for data scientists, integrated with data stores for data flow management with MONAI Label and Core.

============
IT Admin
============

An IT admin’s role is to provision and configure systems to stand up the MONAI Toolkit sandbox to serve an enterprise’s data science and research teams. The toolkit provides the perfect base for those teams to get started quickly with guided tutorials and validated workflows.

***************************
Library Overview
***************************

===============
MONAI Label
===============

MONAI Label minimizes the need for developers and researchers to manually annotate data by providing an intelligent imaging labeling and learning SDK that can be integrated into either customized or template-based data labeling apps. MONAI Label saves developers time, helping them quickly progress to training, tuning, and validating their medical AI models within the MONAI standardized paradigm.

The industry’s most popular open source viewers already have MONAI integrated: 3D Slicer, OHIF, QuPath, Digital Slide Archive, and CVAT, and it is also integrated into cloud service providers. Developers can also incorporate MONAI Label into their custom viewer using server and client APIs, which are well abstracted and documented for seamless integration.

MONAI Label has enhanced active learning capabilities, which is a process that aims to use the least amount of data to achieve the highest possible model performance. Choosing data that will have the most significant influence on your overall model accuracy allows human annotators to focus on the annotations that will have the highest impact on the model performance. Developers can see up to a 75% reduction in training costs with active learning in MONAI Label with increased labeling and training efficiency while achieving better model performance.

`MONAI Label Developer Page <https://monai.io/label.html>`__

===============
MONAI Core
===============

MONAI Core gives developers and researchers a PyTorch-driven library for deep learning tasks that includes domain-optimized capabilities they need for developing medical imaging training workflows. Performance features such as MONAI Core’s AutoML, Smart Caching, GPU-accelerated I/O, and transforms take training from days to hours, and hours to minutes, helping users accelerate AI into clinical production.

With Auto3D segmentation, developers can train models with 1-5 lines of code that can quickly segment regions of interest in data from 3D imaging modalities like CT and MRI, reducing training time from weeks/months to 2 days. And MONAI Core’s federated learning client algorithm APIs are exposed as an abstract base class for defining an algorithm to run on any federated learning platform. NVIDIA FLARE has already built the integration piece with these new APIs. And using MONAI Bundle configurations with the new federated learning APIs means developers can take any bundle and seamlessly extend them to a federated paradigm.

`MONAI Core Developer Page <https://monai.io/core.html>`__

===============
NVIDIA FLARE
===============

NVIDIA FLARE (NVIDIA Federated Learning Application Runtime Environment) is a domain-agnostic, open-source, extensible SDK that allows researchers and data scientists to adapt existing ML/DL workflows (PyTorch, RAPIDS, Nemo, TensorFlow) to a federated paradigm. It enables platform developers to build a secure, privacy-preserving offering for a distributed multi-party collaboration. Built on a componentized architecture, NVIDIA FLARE gives you the flexibility to take federated learning workloads from research and simulation to real-world production deployment.

MONAI includes the federated learning client algorithm APIs exposed as an abstract base class for defining an algorithm to run on any federated learning platform. NVIDIA FLARE has already built the integration piece with these new APIs.

`NVIDIA FLARE Developer Page <https://developer.nvidia.com/flare>`__