项目逻辑：

项目旨在通过对新闻文本进行情感分类，使文本公告转换为情感特征，结合其他指标对后一天的收盘价数据进行预测。

首先对新闻公告文本进行处理，根据word2vec/bert预训练方法将文本进行情感分类（积极，消极，中立），将训练好的情感标签结合股票当天的开盘价，收盘价，最高价，最低价，成交量，时间，股票代码
这几个特征进行机器学习/深度学习预测第二天股票的涨跌情况（涨，跌，平），进行对比实验看哪种模型具有更好的预测效果，并看情感特征是否会增加预测的精度。

详细步骤介绍：

原始数据：
原始数据是从东方财富网得到的公告，网站为 https://data.eastmoney.com/notices/ ，数据日期为2022/5/17-2022/5/22，数据格式如下






