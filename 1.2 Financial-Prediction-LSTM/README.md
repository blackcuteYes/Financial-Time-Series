**基于LSTM预测股票价格（简易版）**

**数据集：**

沪深300数据

**数据特征：**

只选用原始数据特征（开盘价、收盘价、最高价、最低价、交易量）

**时间窗口：**

15天

**代码流程：**

读取数据->生成标签(下一天收盘价)->分割数据集->LSTM模型预测->可视化->预测结果评估

**LSTM网络结构：**

<img src="https://github.com/jm199504/Financial-Prediction/blob/master/Financial-Prediction-LSTM/images/lstm_model.png" width="500">

<img src="https://github.com/jm199504/Financial-Prediction/blob/master/Financial-Prediction-LSTM/images/lstm_model2.png" width="500">

**函数介绍：**

1、generate_label 生成标签（下一天收盘价） 

2、generate_model_data 分割数据集 

3、evaluate 结果评估 

4、lstm_model LSTM预测模型 

5、main 主函数（含可视化）

**可视化输出：**

训练集拟合效果：

<img src="https://github.com/jm199504/Financial-Prediction/blob/master/Financial-Prediction-LSTM/images/train.png">

测试集拟合效果：

<img src="https://github.com/jm199504/Financial-Prediction/blob/master/Financial-Prediction-LSTM/images/test.png">

**评估指标：**

1、RMSE：55.93668241713906

2、MAE：44.51361108752264

3、MAPE：1.3418267677320612

4、AMAPE：1.3420384401412058
