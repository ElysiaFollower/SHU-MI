## 数据

使用数据来自论文A large EEG dataset for studying cross-session variability in motor imagery brain-computer interface
相应文件结构为
./data/
  |-- train/
  |-- val/
使用的是论文给出的.mat文件
其中前20个受试者的数据放在train文件夹下
后5个受试者的数据放在val文件夹下

考虑到数据集占存储空间较大，这里不附上数据集。只要保持上述文件结构即可使用。data文件夹在根目录下。

## 文件



data_exploere.ipynb 用于数据探索

data_preprocess.ipynb用于数据的预处理

train.ipynb用于模型的训练和评估



## 使用



使用data_preprocess.ipynb的主循环部分，设置输入路径和输出路径，对数据进行预处理，得到预处理后的数据。

- 输出文件夹格式：在原始文件夹后面加上“-processed"后缀

- 如要复刻原过程，应当把所有数据文件都放在all文件夹中，然后额外生成一个all-processed文件夹

在train.ipynb中

只需要通过修改pipeline_name变量即可应用不同的机器学习算法。