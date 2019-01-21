# 利用Python挖掘Twitter数据
## 推特数据采集
推特官方提供的API可以让我们获取到所需的数据。  
为此，我们需要推特账号去创建一个app以获得keys和sccess tokens。然后使用Python的Tweepy库来和API交互。在即时任务中可以通过Stream API获取twitter流数据，因为是及时获取的数据，实际速率取决于设置关键词的数量和热门程度，一般不会超出限制。常规任务中可以通过Search API获取twitter历史数据，不过只能够下载当前时间以前的7天的数据，且存在速率限制。两者在[Collecting Tweets with Tweepy](https://github.com/Observer-L/Mining-Twitter-Data-with-Python/tree/master/Collecting%20Tweets%20with%20Tweepy)中有相关的实现。  
BTW，我们还可以在Github或Kaggle上可以找到现有的名人或事件的社交平台数据集，本项目数据来源于[Trump Twitter Archive](trumptwitterarchive.com)，基本涵盖了川普开通推特账号以来的所有推文（2009~），而且持续更新，cool~

## 特朗普的推特文本挖掘
你可以在[Trump Tweets Mining](https://github.com/Observer-L/Mining-Twitter-Data-with-Python/blob/master/Trump%20Tweets%20Mining/Text%20analysis%20of%20Trump's%20tweets.ipynb)中查看全部代码。  
[**到我的博客阅读此文章**](https://observer-l.github.io/project/mining-twitter-data-with-python)以查看更多分析和图表说明，来看看川普这个人那些事儿吧~  

## 参考资料
1. Twitter的[开发者文档](https://dev.twitter.com/rest/public/rate-limiting)  
2. Tweepy的[说明文档](http://docs.tweepy.org/en/v3.5.0/)   
3. Dealing Data [PoGo Series](http://www.dealingdata.net/2016/07/20/PoGo-Series-Intro/)    
4. David Robinson [Text analysis of Trump's tweets confirms he writes only the (angrier) Android half](http://varianceexplained.org/r/trump-tweets/)  
5. Marco Bonzanini [Mining Twitter Data with Python](https://marcobonzanini.com/2015/03/02/mining-twitter-data-with-python-part-1/)  
6. DATAQUEST [Working with streaming data: Using the Twitter API to capture tweets](https://www.dataquest.io/blog/streaming-data-python/)  
[Up-to-date Archive of Trump Tweets](http://www.trumptwitterarchive.com/)
