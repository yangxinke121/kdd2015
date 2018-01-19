# kddcup2015

参考了   https://github.com/its-fun/kddcup2015

## project structure

```
|
|- data/  # 由于数据量很大，因此应该自己创建这个文件夹，并且将数据文件按照这个结构放好
   |- cache/  # pickle dump出来的对象，用于加快文件读取速度
   |- test/  # 测试数据
      |- enrollment_test.csv
      |- log_test.csv
   |- train/  # 训练数据
      |- enrollment_train.csv
      |- log_train.csv
      |- truth_train.csv
   |- object.csv
|- path_config.py  # 与数据路径相关的配置
|- modeling_config.py  # 与模型训练相关的配置
|- dataset.py  # 生成数据集的相关方法
|- feature_extraction.py  # 提取特征的相关方法
|- util.py  # IO等辅助性的工具
|- modeling.py  # 建模的方法
```

Run `python3 dataset.py` to load the dataset


之后运行 modeling.py 进行预测

代码亲测可用，运行两个小时左右.
