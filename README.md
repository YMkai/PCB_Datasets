# PCB Dataset

本PCB数据集包括三部分：

- AOI_Dataset
- Defect_Classification_Dataset
- Spot_Detection_Dataset

## AOI Dataset

原始AOI图像数据，包括三部分：

- PCB：原始AOI光源下拍摄的整版大分辨率图像
- ELEMENGR：瑕疵焊点局部图像
- TEMP：缺陷元器件局部图像

## Defect Classification Dataset

根据北京大学智能机器人开放实验室开放的[印刷电路板（PCB）瑕疵数据集](http://robotics.pkusz.edu.cn/resources/dataset/)切割处理后，只针对分类场景的缺陷分类数据集。

|       缺陷类别        | 图像数量 | 目标数量 |
| :-------------------: | :------: | :------: |
|  缺孔  missing hole   |   115    |   497    |
|   鼠咬  mouse bite    |   115    |   492    |
|  开路  open circuit   |   116    |   482    |
|      短路  short      |   116    |   491    |
|      毛刺  spur       |   115    |   488    |
| 假铜  spurious copper |   116    |   503    |

## Spot Detection Dataset

AOI Dataset原图数据为基础，经过切割标注后得到的目标检测数据集。

其中训练集含948个416×416的图像，测试集分为416×416、832×832、1024×1024大小。