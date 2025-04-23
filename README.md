# Requirements to test and wrap gpu tool for Galaxy

## Installation
1) ensure nvidia-smi is installed
2) ensure nvcc is installed
3) ensure the nvidia driver is installed on windows if ubuntu WSL is used

##  Install Graphics Card Drivers
Visit the official NVIDIA website to download [NVIDIA DRIVER](https://www.nvidia.com/es-es/drivers/) and fill in the fields with the corresponding graphics card and OS information. Download the driver and run the file to install the driver on Windows OS.

## Install NVIDIA drivers in WSL
Start the Ubuntu terminal and run the folowing command to update the packages.
```
sudo apt update && upgrade
```
Then, install the nvidia drivers according to the version. In this example, we installed version 555 on ubuntu 22.04.
```
wget https://developer.download.nvidia.com/compute/cuda/12.5.0/local_installers/cuda_12.5.0_555.42.02_linux.run
sudo ./cuda_12.5.0_555.42.02_linux.run
or
sudo apt install cuda-toolkit-12-5
```
