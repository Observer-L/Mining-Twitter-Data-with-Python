# 利用Python挖掘Twitter数据

### 数据采集
推特官方提供的API可以让我们获取到所需的数据。  
为此，我们需要推特账号去创建一个app以获得keys和sccess tokens。然后通过Python里的Tweepy包来和API交互。在CSDN或一些技术博客里可以找到关于这方面的内容。  
在即时任务中可以通过Stream API获取twitter流数据，因为是及时获取的数据，实际速率取决于设置关键词的数量和热门程度，一般不会超出限制。常规任务中可以通过Search API获取twitter历史数据，不过只能够下载当前时间以前的7天的数据，且存在速率限制。两者在Collecting Tweets with Tweepy中有相关的实现。  
Btw，在Github上可以找到一些名人推特的数据集，例如[特朗普的推特数据集](https://github.com/bpb27/trump_tweet_data_archive)。

### 特朗普的推特文本挖掘
我利用一个现有且不错的特朗普推特数据集对特朗普的推特进行了一些较为基础的分析，你可以在[Trump Tweets Mining](https://github.com/Observer-L/Mining-Twitter-Data-with-Python/blob/master/Trump%20Tweets%20Mining/Text%20analysis%20of%20Trump's%20tweets.ipynb)中查看全部代码，在此[文章](http://linliphotography.com/mining-twitter-data-with-python/)中查看我的分析过程和结论。  


### 参考资料
Twitter的[开发者文档](https://dev.twitter.com/rest/public/rate-limiting)  
Tweepy的[说明文档](http://docs.tweepy.org/en/v3.5.0/)   
Dealing Data [PoGo Series](http://www.dealingdata.net/2016/07/20/PoGo-Series-Intro/)    
David Robinson [Text analysis of Trump's tweets confirms he writes only the (angrier) Android half](http://varianceexplained.org/r/trump-tweets/)  
DATAQUEST [Working with streaming data: Using the Twitter API to capture tweets](https://www.dataquest.io/blog/streaming-data-python/)  
[Up-to-date Archive of Trump Tweets](http://www.trumptwitterarchive.com/)
