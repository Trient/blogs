## PHP:Excel:Export
> #### 有意思的代码片段:
>> openXML
>>>
   - 数据内```<>```符号要用 ```&lt;&gt;``` 替换，否则会因为无闭合标签出错；

>> CSV
>>>
   - 注意过滤英文逗号, 否则换行错乱

>> 数据量大、请求数少
>>> 可用协程，推荐队列

>> 数据量大、请求数多(如SAAS平台)
>>> 队列导出、上传CDN、邮件发送下载链接