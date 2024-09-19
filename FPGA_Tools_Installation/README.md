### Vitis 2023.2 Installation

* Installation Requirements
  * The Vitis™ software platform consists of an integrated development environment (IDE) for interactive project development, and command-line tools for scripted or manual application development. The Vitis software platform also includes the Vivado® Design Suite for implementing the kernel on the target device, and for developing custom hardware platforms.
  * Note: Windows OS support is limited to the Vitis embedded software development flow. The acceleration features in the Vitis software platform are not supported.

---
### Embedded Software Development Flow 

* Minimum System Requirements
  * To install and run on a computer, your system must meet the following minimum requirements.

<img src="https://github.com/user-attachments/assets/104abffd-4d34-4501-9506-0dd122ea9f1d" width="600">

---
### Installing the Vitis 2023.2 Software Platform

* https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vivado-design-tools/2023-2.html 

<img src="https://github.com/user-attachments/assets/e908d169-53fe-4fd5-b81f-cc40735e1672" width="800">

---
1. Go to the Xilinx Downloads Website [[link]](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/vitis/2023-2.html).
2. Download the installer for your operating system.
3. Run the installer, which opens the Welcome page of the Xilinx Unified 2023.2 Installer.
4. Click Next to open the Select Install Type page of the Installer.
5. Enter your Xilinx user account credentials, and then select Download and Install Now.
6. Click Next to open the Accept License Agreements page of the Installer.
7. Accept the terms and conditions by clicking each I Agree check box.
8. Click Next to open the Select Product to Install page of the Installer.
9. Select Vitis and click Next to open the Vitis Unified Software Platform page of the Installer.
10. Customize your installation by selecting design tools and devices (optional)
11. Click Next to open the Select Destination Directory page of the Installer
12. Specify the installation directory, review the location summary, review the disk space required
13. Click Install to begin the installation of the software

---
### Installing Embedded Platforms
* Embedded platforms are available to download from the [Vitis Embedded Platforms download page](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/embedded-platforms/2023-2.html) for use in the Vitis unified software platform. 

<img src="https://github.com/user-attachments/assets/6b767a69-8c0e-41b7-a4b6-b3a2bea42d9e" width="800">

---

* For the Vitis embedded software development flow, you can use embedded platforms with Linux, standalone/bare metal, or RTOS domains. 
* To support the Vitis application acceleration development flow, embedded platforms must run Linux, with XRT integrated into the rootfs. 
* Some of the supported platforms are listed here. A complete list can be found on the [downloads page](https://www.xilinx.com/support/download/index.html/content/xilinx/en/downloadNav/embedded-platforms/2023-2.html).

<img src="https://github.com/user-attachments/assets/5bf63aa0-6f37-495d-a70c-a2b91698b291" width="450">

---
### Setting Up the Environment to Run the Vitis Software Platform

* To configure the environment to run the Vitis software platform, run the following script in a command shell to set up the tools to run in that shell:
```
# setup XILINX_VITIS and XILINX_VIVADO variables 
$ source <Vitis_install_path>/Vitis/2023.2/settings64.sh 
```

* To use any platforms you have downloaded as described in Installing Embedded Platforms, set the following environment variable to point to the location of the platforms:
```
$ export PLATFORM_REPO_PATHS=<path to platforms>
```
---
### Install Vitis-AI Tools and Resources

Clone Xilinx Vitis-AI Repository
1. Install the docker, ensure Linux user is in the group docker
    
2. Clone the Vitis-AI repository:
```
git clone --recurse-submodules https://github.com/Xilinx/Vitis-AI 
```
3. cd Vitis-AI

* Run the docker container (running on CPU):
```
./docker_run.sh xilinx/vitis-ai-cpu:latest
```
    
* Run the docker container (running on GPU):
``` 
./docker_run.sh xilinx/vitis-ai-gpu:latest
```

4. Get started with examples


