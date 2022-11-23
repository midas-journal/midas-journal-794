### README

This folder contains the source code for VascuSynth project: https://vascusynth.cs.sfu.ca/Welcome.html

Please cite the following two publications if you intend to use the provided code:

---

Ghassan Hamarneh and Preet Jassi. "VascuSynth: Simulating Vascular Trees for Generating           Volumetric Image data with Ground Truth Segmentation and Tree Analysis," Computerized Medical Imaging and Graphics, 2010. [pdf](https://www2.cs.sfu.ca/~hamarneh/ecopy/cmig2010.pdf)

Preet Jassi and Ghassan Hamarneh. "VascuSynth: Vascular Tree Synthesis Software," Insight Journal, 2011. [pdf](http://www.cs.sfu.ca/~hamarneh/ecopy/ij2011.pdf)

---

## Installation Instructions

This software was developed upon an earlier version of [ITK](https://itk.org/). Please make sure you download the 4.13.3 version to your local machine. 

To generate both ITK and VascuSynth projects on generic platforms, you also need a copy of [CMake](https://cmake.org/), you can choose the latest version of CMake with GUI.

To build both ITK projects and VascuSynth projects, you need a copy of C++ compiler in your machine. We recommend Microsoft Visual Studio 2015 Community version for Windows users.

1. Download and unzip ITK to local folder, e.g., /home/ITK
2. Set the generated ITK binaries path to /home/ITK/bin
3. Run configure and Generate
4. Go to /home/ITK/bin, open ITK.sln and build the project (this step is specific for VS 2015).
5. download VascuSynth to local folder, e.g., /home/vascusynth
6. Set ITK_DIR=root/ITK/bin inside CMake and generated bin folder as /home/vascusynth/bin
7. Run configure and Generate
8. Go to home/vascusynth/bin, build VascuSynth.sln
9. The built VascuSynth.exe is under /home/vascusynth/bin/Debug

## Generate Images

Please put all the parameter files in the sample_params folder under  /home/vascusynth/bin/Debug, then run the command line like below:

`./VascuSynth  paramFiles.txt imageNames.txt 0.04`

