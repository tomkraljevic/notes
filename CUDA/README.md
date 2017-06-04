# Random CUDA notes and resources

Install:

* <https://developer.nvidia.com/cuda-gpus>
* <http://docs.nvidia.com/cuda/cuda-installation-guide-mac-os-x/index.html>
* <https://developer.nvidia.com/cuda-downloads>
* <https://developer.nvidia.com/gpu-deployment-kit>

Uninstall:

* <http://docs.nvidia.com/cuda/cuda-installation-guide-mac-os-x/index.html#uninstall>

Pascal chip architecture:

* <https://devblogs.nvidia.com/parallelforall/inside-pascal/>
* <https://developer.nvidia.com/pascal>
* <https://images.nvidia.com/content/pdf/tesla/whitepaper/pascal-architecture-whitepaper.pdf>
* <https://en.wikipedia.org/wiki/Pascal_(microarchitecture)>

Comparison with Xeon Phi:

* <https://en.wikipedia.org/wiki/Xeon_Phi>
* <http://wccftech.com/intel-knights-landing-detailed-16-gb-highbandwidth-ondie-memory-384-gb-ddr4-system-memory-support-8-billion-transistors/>

Books:

* <http://docs.nvidia.com/cuda/pdf/CUDA_C_Programming_Guide.pdf>

Portability:

* <https://devblogs.nvidia.com/parallelforall/developing-portable-cuda-cc-code-hemi/>

Thrust:

* <http://cs.boisestate.edu/~alark/thrust_intro/presentation.html#slide1>

Webinars:

* <https://developer.nvidia.com/gpu-computing-webinars>

Toolchain documentation:

* <http://docs.nvidia.com/cuda/pdf/CUDA_Compiler_Driver_NVCC.pdf>

Management and Performance APIs:

* <https://developer.nvidia.com/nvidia-management-library-nvml>
* <http://docs.nvidia.com/cuda/cupti/index.html>

Unified Memory:

* <https://devblogs.nvidia.com/parallelforall/unified-memory-in-cuda-6/>

---

Idea for how to do predictions on the GPU:

Thrust webinar
Slide 20

---

How to keep temporary files from nvcc

```
nvcc -v -keep -keep-dir tmp
```

---

Install examples:

```
cd
mkdir Cuda
cd Cuda
cuda-install-samples-8.0.sh .
```

Compile and run an example:

```
cd Cuda/NVIDIA_CUDA-8.0_Samples
make -C 1_Utilities/bandwidthTest
./bin/x86_64/darwin/release/bandwidthTest
```