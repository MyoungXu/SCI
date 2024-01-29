
# SCI-低光增强

这个工程记录我自己跑通的一些代码，并介绍怎么在自己电脑上运行。


原文章可以在这里找到：
[CVPR 2022 Open Access Repository (thecvf.com)](https://openaccess.thecvf.com/content/CVPR2022/html/Ma_Toward_Fast_Flexible_and_Robust_Low-Light_Image_Enhancement_CVPR_2022_paper.html?ref=https://githubhelp.com)
  
原代码可以在[这里](https://github.com/vis-opt-group/SCI)找到：

## 环境

* 建议使用python3.7
* 我自己用的torch版本
```bash
conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch
```
* 没有其他需要安装的库

## 输入数据格式

我建议在`./data`中创建一个自己的文件夹（比如：`./data/FOLDER`），然后将所有需要处理的图像放进该文件夹即可。

**注意！该工程仅处理png格式的数据，如果输入其他格式可能会导致无法正常输出结果！**

  

## 运行

运行该工程非常简单。只需要在终端运行：
```bash
python test.py --data_path data/FOLDER --save_path results/FOLDER
```
如果你想要在本地简单运行，直接修改`test.py`中第14行的地址为`FOLDER`即可。
