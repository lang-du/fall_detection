# 基于yolo的摔倒检测
将Aistudio一个项目部署部分提取出来，仅保留部署所需的代码，完整代码参考项目链接。  
项目连接：[https://aistudio.baidu.com/aistudio/projectdetail/2500639?channelType=0&channel=0](https://aistudio.baidu.com/aistudio/projectdetail/2500639?channelType=0&channel=0)   

## 一、介绍
本项目基于深度学习框架paddlepaddle，使用yolov3目标检测算法实现任务摔倒检测，检测效果如下图。  
![detected_result](output/people_930.jpg)

## 二、目录
|-images  存放待检测的图片  
|-output  存放检测好的图片  
|-yolov3_mobilenet_v3_large_voc  存放模型权重文件    

## 三、环境
paddlepaddle>=2.0.0  

## 四、快速使用
1、安装paddle2.0.0以上版本
```bazaar
pip install paddlepaddle
```
2、安装依赖库 
```bazaar
pip install -r requirements.txt
```
3、运行检测，检测结果在output目录中  
```bazaar
python .\infer.py --model_dir=yolov3_mobilenet_v3_large_voc --image_file=images\people_930.jpg
```

## 五、其他
目标检测、语义分割模型定制，联系QQ：884001583