# Repository for Tensorflow 1.11.0-rc1 

Tensorflow 1.11.0-rc1 compiled from source to only support GPU usage on Debian 9 Stretch


## Installation

`pip3 install tensorflow-1.11.0rc1-cp36-cp36m-linux_x86_64.whl`


## Environment

| Component | Version |
| :-------------: | :-------------: |
| Distro   | `Debian 9 (Stretch)`   |
| Kernel   |  `linux-image-4.9.0-8-amd64`   |
| GPU / Compute Capcity     |  `Nvidia GeForce GTX 1080 TI` / `6.1`  |
| Tensorflow   |  `v1.11.0 rc1`   |
| CUDA   |  `9.1.85-4+b1 amd64`   |
| cuDNN   |  `7.1.3`   |
| NCCL   |  `2.1.15`   |
| GCC   |  `gcc-6`   |
| Python   |  `3.6.6`   |
| Bazel   |  `0.17.0`   |
| Tested against NVIDIA Driver Runtime   |  `390.77`   |



## Bazel Configure file 

```
Please specify the location of python. [Default is /usr/bin/python]: 
/usr/bin/python3


Please input the desired Python library path to use.  Default is [/usr/local/lib/python3.6/dist-packages]

/usr/local/lib/python3.6/dist-packages


Do you wish to build TensorFlow with jemalloc as malloc support? [Y/n]: Y

jemalloc as malloc support will be enabled for TensorFlow.


Do you wish to build TensorFlow with Google Cloud Platform support? [Y/n]: n

No Google Cloud Platform support will be enabled for TensorFlow.


Do you wish to build TensorFlow with Hadoop File System support? [Y/n]: n

No Hadoop File System support will be enabled for TensorFlow.


Do you wish to build TensorFlow with Amazon AWS Platform support? [Y/n]: n

No Amazon AWS Platform support will be enabled for TensorFlow.


Do you wish to build TensorFlow with Apache Kafka Platform support? [Y/n]: n

No Apache Kafka Platform support will be enabled for TensorFlow.


Do you wish to build TensorFlow with XLA JIT support? [y/N]: n

No XLA JIT support will be enabled for TensorFlow.


Do you wish to build TensorFlow with GDR support? [y/N]: n

No GDR support will be enabled for TensorFlow.


Do you wish to build TensorFlow with VERBS support? [y/N]: n

No VERBS support will be enabled for TensorFlow.


Do you wish to build TensorFlow with nGraph support? [y/N]: n

No nGraph support will be enabled for TensorFlow.


Do you wish to build TensorFlow with OpenCL SYCL support? [y/N]: n

No OpenCL SYCL support will be enabled for TensorFlow.


Do you wish to build TensorFlow with CUDA support? [y/N]: y

CUDA support will be enabled for TensorFlow.



Please specify the CUDA SDK version you want to use. [Leave empty to default to CUDA 9.0]: 9.1


Please specify the location where CUDA 9.1 toolkit is installed. Refer to README.md for more details. [Default is /usr/local/cuda]: 


Please specify the cuDNN version you want to use. [Leave empty to default to cuDNN 7.0]: 7.1.3


Please specify the location where cuDNN 7 library is installed. Refer to README.md for more details. [Default is /usr/local/cuda]: 



Do you wish to build TensorFlow with TensorRT support? [y/N]: n

No TensorRT support will be enabled for TensorFlow.


Please specify the NCCL version you want to use. If NCCL 2.2 is not installed, then you can use version 1.3 that can be fetched automatically but it may have worse performance with multiple GPUs. [Default is 2.2]: 2.1.15


Please specify the location where NCCL 2 library is installed. Refer to README.md for more details. [Default is /usr/local/cuda]:/usr/local/cuda/nccl


Please specify a list of comma-separated Cuda compute capabilities you want to build with.

You can find the compute capability of your device at: https://developer.nvidia.com/cuda-gpus.

Please note that each additional compute capability significantly increases your build time and binary size. [Default is: 3.5,7.0]: 6.1



Do you want to use clang as CUDA compiler? [y/N]: n

nvcc will be used as CUDA compiler.


Please specify which gcc should be used by nvcc as the host compiler. [Default is /usr/bin/x86_64-linux-gnu-gcc-8]: /usr/bin/gcc-6	



Do you wish to build TensorFlow with MPI support? [y/N]: n

No MPI support will be enabled for TensorFlow.

Please specify optimization flags to use during compilation when bazel option "--config=opt" is specified [Default is -march=native]: 


Would you like to interactively configure ./WORKSPACE for Android builds? [y/N]: n

Not configuring the WORKSPACE for Android builds.

Preconfigured Bazel build configs.

```

## Thanks

  - github user metral for the table structure
  - https://medium.com/@asmello/how-to-install-tensorflow-cuda-9-1-into-ubuntu-18-04-b645e769f01d

