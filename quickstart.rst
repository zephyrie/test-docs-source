####################
Quickstart Guide
####################

************************************************
Running the MONAI Toolkit JupyterLab Instance
************************************************

To start with a local host system, the MONAI Toolkit JupyterLab instance can be started with a ready-to-open website link with:

::

   docker run --gpus all -it --rm --ipc=host --net=host nvcr.io/nvidia/clara/monai-toolkit /opt/docker/runtoolkit.sh

After the JupyterLab App is started, follow the onscreen instruction and open the URL in a web browser.

**Note:** By default, the container use the host system’s all GPU resources, networking and inter-process communication (IPC) namespace. Multiple notebooks require a large shared memory size for the container to run comprehensive workflows. For more information, please refer to `changing the shared memory segment size <#1.4-Changing-Shared-Memory-Segment-Size>`__

************************************************
Running the MONAI Toolkit in Interactive Bash
************************************************

To run the MONAI Toolkit container with the bash shell, issue the command below to start the prebuilt container:

::

   docker run  --gpus all -it --rm --ipc=host --net=host \
               nvcr.io/nvidia/clara/monai-toolkit \
               /bin/bash

************************************************
Changing Shared Memory Segment Size
************************************************

`DIGITS <https://developer.nvidia.com/digits>`__ uses shared memory to share data between processes. For example, if you use Torch multiprocessing for multi-threaded data loaders, the default shared memory segment size that the container runs with may not be enough. Therefore, you should increase the shared memory size by issuing either:

::

   --ipc=host

or

::

   --shm-size=


************************************************
Access the JupyterLab Remotely
************************************************

Users can access the JupyterLab instance by simply typing the host machine’s URL or IP address in the web browser with the port number (default: 8888). A token may be required to log in for the first time. Users can find the token in the system which hosts the MONAI Toolkit container by looking for the code after ``/?token=`` on the screen.


**********************************************************
Running the JupyterLab Instance on a Remote Host Machine
**********************************************************

JupyterLab is started on port 8888 by default. If the user wants to assign another port, the JupyterLab instance can be started by setting the ``JUPYTER_PORT`` environment variable:

::

   -e JUPYTER_PORT=8900

For example:

::

   docker run  --gpus all -it --rm --ipc=host --net=host \
               -e JUPYTER_PORT=8900 \
               nvcr.io/nvidia/clara/monai-toolkit \
               /opt/docker/runtoolkit.sh

**Note:** More details about running docker commands are explained in the `Running A Container <https://docs.nvidia.com/deeplearning/frameworks/user-guide/index.html#runcont>`__ chapter in the NVIDIA Containers For Deep Learning Frameworks User’s Guide and specify the registry, repository, and tags.

********************************
Mount Custom Data Directory
********************************

To mount a custom data directory, the users can use ``-v`` to mount the drive(s) and override the default data directory environment variable ``MONAI_DATA_DIRECTORY`` used by many notebooks. For example:

::

   docker run  --gpus all -it --rm --ipc=host --net=host \
               -v ~/workspace:/workspace \
               -e MONAI_DATA_DIRECTORY=/workspace/data \
               nvcr.io/nvidia/clara/monai-toolkit \
               /opt/docker/runtoolkit.sh

*************************
Configure JupyterLab
*************************

``/opt/docker/runtoolkit.sh`` provides an entry point for the user to configure Jupyter Lab with the default settings. However, it cannot cover all use scenarios and APIs of Jupyter. The user can run the Jupyter Lab command in the MONAI Toolkit container and configure the instance simply by:

::

   docker run --gpus all -it --rm --ipc=host --net=host nvcr.io/nvidia/clara/monai-toolkit jupyter lab

