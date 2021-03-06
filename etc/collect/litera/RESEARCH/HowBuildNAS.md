## 如何构建NAS系统
> 时间: 2018年9月28日

最近碰到一个需求: 由于不可描述的原因, 国内没有好的正版蓝光/4k影视商城, 好多资源都需要自行寻找资源->然后下载(这点游戏就好很多了, 至少在xbox/ps-store/steam购买后, 不管什么时候都能下载, 正版的好处之一). 对于大多数比较好的电影, 我希望是存下来, 然后下次就不用再费力去寻找了. 此时就会有一个问题, 存到哪里合适.

首先, 考虑云盘. 先说结论, 同步盘比较贵但是安全性很高, 备份盘比较便宜但是容易变成8秒教育片.
1. 备份盘: 侧重容量的云盘, 如百度云, 115. 不客气的说, 国内绝大多数云盘存储的资源都存在很大的几率变成8秒教育片, 如BD云盘, 115最近也不行了, 其他的更不用说, 迅雷也自废武功.
2. 同步盘: 侧重安全的云盘, 第三方同步盘推荐坚果云. 其实大多数OS自带的就已经足够使用了, 如IOS自带的icloud, win的onedrive. 只是需要跨平台存储活着同步办公的数据需要第三方云盘, 目前国内推荐坚果云, 算是不错的同步盘了.

其次, 考虑使用阿里/腾讯/AWS等云计算公司的归档存储/对象存储/文件存储(OAS/OSS/NAS)等服务. 土豪优选
1. [OSS优势参考](https://www.alibabacloud.com/help/zh/doc-detail/31817.htm)
2. 简单总结, OSS的优点是 安全可靠, 下载/上传网速快, 且拥有数据处理能力, 可编程, 有API接口. OSS的缺点基本上只有一个: 因为只能通过 客户端/API 上传/下载, 所以不能自动同步, 需要设计相应的程序.
3. 不推荐OSS/NAS的原因, 主要是因为太贵了. OSS存储 1T/年 需要 1000, NAS两千多, 而且 OSS外网流出费用 0~8点 0.25元/G, 其他时间 0.5元/G, 还是比较贵的.
    - PS: 现在阿里云在打折, 1T 3年 中国大陆的, 只要99...
4. OAS/OSS/NAS 还是比较适合企业/建站使用的, 个人使用太不值了, 好多价值发挥不出来.

最后, 就是自搭NAS(Network Attached Storage), 扩展最丰富的, 也是最能折腾的.
1. [自建NAS参考](https://www.zhihu.com/question/21359049)
2. 其实NAS就是一台本地的低功耗/偏向存储功能的服务器. 可以自己查阅常用NAS的配置, 然后自己根据需求组装一个.

## 参考
- [磁力链接是如何实现下载的](http://www.aneasystone.com/archives/2015/05/how-does-magnet-link-work.html)
