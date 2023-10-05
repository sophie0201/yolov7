## 我的實驗環境
- windows 10
- GeForce840M
- 最高版本: CUDA 9.1.83 
## cuda install & cudnn install
- cuda: https://developer.nvidia.com/cuda-90-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exenetwork
- 加入環境變數->系統變量>path: C:\Program Files\NVIDIA Corporation\NVSMI
- 檢查: nvidia-smi,nvcc -V, set cuda(加入環境變數) [https://codeantenna.com/a/PMzSaPMlg8]
- cudnn 7.6.5: https://developer.nvidia.com/rdp/cudnn-archive
## conda env setup
- conda create --name torch python=3.7
- ![image](https://github.com/sophie0201/yolov7/assets/126761277/6a701010-3866-40ff-a620-67b3c6e1b2f6)
- CUDA 9.0
`conda install pytorch==1.0.1 torchvision==0.2.2 cudatoolkit=9.0 -c pytorch`
- torchvision: `pip install  torchvision==0.2.2`(因為conda沒有這麼舊版本)
- torch: `pip install torch-1.0.1-cp37-cp37m-win_amd64.whl` [https://download.pytorch.org/whl/cu90/torch_stable.html]
## yolov7 setup
- 註解torch、torchvision
- `pip install -r requirements.txt`
- `python test.py --data data/coco.yaml --img 640 --batch 32 --conf 0.001 --iou 0.65 --device 0 --weights yolov7.pt --name yolov7_640_val`
- 結果:![image](https://github.com/sophie0201/yolov7/assets/126761277/6e849872-fd2b-4bbb-8b66-14f0ba220448)
- 搞了1天，哭了
- 只能上colab


