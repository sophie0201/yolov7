## 我的實驗環境
- windows 10
- GeForce840M
- 最高版本:CUDA 9.1.83 
## cuda install & cudnn install
- cuda: https://developer.nvidia.com/cuda-90-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exenetwork
- 加入環境變數->系統變量>path:C:\Program Files\NVIDIA Corporation\NVSMI
- 檢查:nvidia-smi,nvcc -V, set cuda[https://codeantenna.com/a/PMzSaPMlg8]
- cudnn:
## conda env setup
- conda create --name torch python=3.8
