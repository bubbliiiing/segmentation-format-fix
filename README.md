## Segmentation Format Fix-该仓库中放置了一些工具，用于调整语义分割算法的数据集格式，使其符合训练要求。
---

## 目录
1. [原图处理](#原图处理)
2. [标签处理](#标签处理)

## 原图处理
在本人提供的一些语义分割仓库中，当输入的原图后缀不为.jpg时无法正常训练，可使用Convert_JPEGImages.py进行原图后缀批量修改。
### 修改步骤
1、Origin_JPEGImages_path用于指定需要修改后缀的图片汇总；    
2、Out_JPEGImages_path用于指定输出的图片路径；    
3、修改后运行，批量处理原图，处理为RGB图并将后缀改为.jpg。   

## 标签处理
在本人提供的一些语义分割仓库中，标签的每个像素点的值就是这个像素点所属的种类，如果不符合的话则会没有训练效果。可使用Convert_SegmentationClass.py进行标签批量修改。
### 修改步骤
1、Origin_SegmentationClass_path用于指定需要修改的标签汇总；   
2、Out_SegmentationClass_pathh用于指定输出的标签路径；   
3、Origin_Point_Value用于指定原始标签所在的路径；   
4、Out_Point_Value用于指定输出标签对应的像素点值；   
5、修改后运行，批量处理标签，处理为png灰度图。  