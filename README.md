# Attention-based Neural Collaborative（ANC）

## 说明

## 环境说明
- pytorch version: '1.9.0'
- python version: '3.8'

## 代码运行

Run ANC:

```
python main.py
```


## 参数说明

- 将模型使用的参数放置在 utils/config.py 中


## 数据集

data/gowalla 数据说明：
- groupMember.csv
  - 每一行包含的数据格式为：群组id, 工人id1, 工人id2,..
- groupNegative.csv
    - 每一行包含的数据格式为：群组id, 任务id, 负采样的任务id1,负采样的任务id2,...
    - 每一行的负样本包含50个
    - 负采样的任务ID表示群组内工人没有执行过的任务
- groupTest.csv
    - 每一行有两个数据分别表示：群组ID，任务ID
- groupTrainNew.csv
    - 每一行有两个数据分别表示：群组ID，任务ID
- userNegative.csv
    - 每一行包含的数据格式为：群组id, 任务id, 负采样的任务id1,负采样的任务id2,...
    - 每一行的负样本包含50个
    - 负采样的任务ID表示工人没有执行过的任务
- userTest.csv
    - 每一行有两个数据分别表示：工人ID，任务ID
- userTrainNew.csv
    - 每一行有两个数据分别表示：工人ID，任务ID
- userSensor.csv
    - 每一行分别表示：工人ID，工人带有的传感器id1, id2,...