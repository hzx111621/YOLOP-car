# YOLOP-car
 基于YOLOP的车道检测和距离检测系统
 
<img width="1280" alt="屏幕截图 2024-10-12 170918" src="https://github.com/user-attachments/assets/88271cf5-e69b-471a-b9b0-ee67039b12fe">

主要原理基于华中科技大学团队开源的YOLOP项目（项目地址：https://github.com/hustvl/YOLOP）

在此基础上添加了单目距离计算用以计算与牵扯的距离，并作出相应提醒。

同时调整了代码，使其可以在NVIDIA RTX3060 上利用CUDA进行加速计算。

PYTHON版本：3.7

TORCH版本：cu111/torch-1.8.0%2Bcu111-cp37-cp37m-win_amd64.whl

# 安装依赖
pip3 install -r requirements.txt

# 运行测试

# 视频文件测试
python tools/demo.py --source test.mp4  --device 0

# 图像文件测试
python tools/demo.py --source test.jpg  --device 0

# 摄像头测试
python tools/demo.py --source 0   --device 0     

