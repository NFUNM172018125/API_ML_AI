# 数英小圆通

| 发布日期 | 2019年12月 | 
| :------| ------: | 
| 产品名称 | 数英小圆通 | 
| 文件现状 | 正在更新 | 
| 领头的设计师 | 黄舒静 | 
| 领头的开发者 | 黄舒静 | 


### 第一部分
#### 一、加值宣言
##### 学而思网校AI开放平台OCR速算API的价值
* 自动识别图片中的速算题并进行智能检查是否正确，有效帮助家长摆脱繁琐的检查作业工作。

##### 学而思网校AI开放平台OCR文字识别的价值
* 将图片中文本快速转换成可编辑的文字。

##### 讯飞语音合成API的价值
* 将文字信息转化为声音信息，帮助用户快速获取文字的读音。

##### 百度AI拍照翻译SDK的价值
* 将图像识别与文本翻译合二为一，轻松实现图文翻译，帮助用户快速获取文本翻译。

### 二、用户需求
* 家长检查孩子数学题时，但孩子数学作业多，看数字眼花缭乱，此时，需要一个软件帮助他们快速判别孩子作业的正确性。
* 家长辅导孩子英语学习，但对一些英语单词的读音存在疑惑，此时家长需要一个软件，帮助他们准确地获取单词的读音，辅导孩子学习。
* 家长辅导孩子英语学习时，对一些单词的中文意思理解不多，此时家长需要一个软件，帮助他们不用手打输入，快速获取单词读音。


### 三、核心价值
最小可行性产品：
* 提供给家长，帮助家长检查孩子的数学作业以及辅导孩子学习英语。

### 四、用户痛点

| 序号 | 痛点 | 
| :------:| :------ | 
| 1 | 家长白天工作，晚上检查孩子作业，需要花费大量的时间检查，劳累过度，容易生气，导致亲子关系紧张 | 
| 2 | 家长辅导孩子英语学习，但不是很清楚地知道一些英语单词的发音 | 
| 3 | 家长辅导孩子英语学习，但对一些英语单词的中文意思存在疑惑 | 

### 五、产品简介
* 该产品提供OCR速算输入为用户拍摄照片或上传本地图片。
* 该产品提供学而思网校OCR识别输入为拍摄照片或上传本地照片，为用户快速获取图片中的文本。
* 该产品可以为用户提供通过OCR获取的文本读音，帮助用户解决不懂发音的问题。
* 该产品可以为提供百度AI拍照翻译SDK，帮助用户快速获取文本翻译信息。

### 六、人工智能概率性
* 拍照速算识别成功率：讯飞达98%[讯飞拍照速算识别](https://www.xfyun.cn/services/photo-calculate-recg)>学而思网校97.5%[OCR速算](https://docai.xueersi.com/books/ai%E6%95%99%E8%82%B2%E5%BC%80%E6%94%BE%E5%B9%B3%E5%8F%B0/page/ocr%E9%80%9F%E7%AE%97)

* 目前百度AI OCR识别整体准确率90%[百度文字识别](https://ai.baidu.com/tech/ocr/general)，而学而思网校开放平台的OCR识别率均在93%以上[https://blog.csdn.net/aiya_y12a/article/details/88955072](https://blog.csdn.net/aiya_y12a/article/details/88955072)

### 七、需求列表与人工智能加值

| 优先级 | 用户需求 | 功能 | 
| :------:| :------ | :------: | 
| 重要 | 用户需要节省时间检查孩子的作业，提高工作效率 | OCR速算 | 
| 重要 | 用户需要将图片的文字转换为可编辑的文本文字，提高辅导效率，同时解决用户不想手打输入的问题 | OCR文字识别 | 
| 重要 | 用户需要将文字识别后的文本以语音的方式输出，获取文字的读音，解决用户辅导过程中遇到不熟悉的英文单词读音的问题 | 语音合成 | 
| 次重要 | 用户想要快速获取一段文本或是单词的中文意思，节省手打时间 | 拍照翻译SDK | 

### 第二部分 原型

### 第三部分 产品使用关键AI或机器学习之API的输出入展示
##### API使用水平
* 学而思网校开放平台OCR速算API [详细代码示例]()
* 学而思网校开放平台OCR文字识别API [详细代码示例]()
* 讯飞语音合成API [详细代码示例]()
* 百度AI拍照翻译SDK API [详细代码示例]()
* API使用比较分析

##### 使用比较分析

##### 速算API比较
* 讯飞开放平台和学而思网开放平台的速算识别api准确率均在97%以上。

| 对比平台 | 讯飞 | 学而思 | 
| :------:| :------ | :------: | 
| 代码比较 | [讯飞拍照速算识别详细代码]() | [学而思OCR速算详细代码]() | 
| 使用效果 | 对于文字识别准确率相对低，不能准确识别一些手写体或是数学单位，识别时间快 | 文字识别准确率高，但识别时间相对慢 | 
| 成熟度 | [官方文档有详细的demo](https://www.xfyun.cn/doc/words/photo-calculate-recg/API.html#%E8%B0%83%E7%94%A8%E7%A4%BA%E4%BE%8B) | [官方文档有详细的demo](https://docai.xueersi.com/books/ai%E6%95%99%E8%82%B2%E5%BC%80%E6%94%BE%E5%B9%B3%E5%8F%B0/page/ocr%E9%80%9F%E7%AE%97) | 
| 性价比 | 每日100000次限额，可申请提额 | 每日限额100000 | 
| 服务评估 | 有api文档且有示例代码，更换APPID、APISecret、APIKey即可用，便于使用，识别时间快，但准确率有待提升 | 有api文档且有示例代码，更换更换APPID、APISecret、APIKey即可用，便于使用，准确率高于讯飞，但识别时间慢 | 





