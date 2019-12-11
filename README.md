# 植物通

| 发布日期 | 2019年12月 | 
| :------| ------: | 
| 产品名称 | 植物通 | 
| 文件现状 | 未完成 | 
| 领头的设计师 | 黄舒静 | 
| 领头的开发者 | 黄舒静 | 
| 迭代版本 | 1.0  | 

### 背景
植物园是我们日常生活欢乐时光或者是增长知识的场所，大部分植物园会在某一区对植物进行基础信息的介绍，但是对于植物的详细介绍十分少。我们在植物园游玩时总会遇到一些不认识的植物，且身边的朋友不懂，但是此时人流量多，无法查看植物园信息区对植物的介绍。如果有一个植物识别app给予用户解说，同时提供植物所在的位置信息，给予用户路径规划，将会提高游客的观赏体验。

### 产品市场
目前市场上已经有相类似的植物识别app，上传照片进行识别得到对应植物信息，例如“自然观察”app。但此类app大多功能单一，只能简单的对植物进行识别，且当照片中存在人物时无法识别植物。运用百度AI植物识别api和路径规划api，帮助用户获取植物信息的同时为用户提供到达植物园区的路径规划。

### 加值宣言
运用百度AI中动物识别api,拍下任意植物照片，输出照片植物的百度百科详细信息，运用高德地图路径规划api，在输入不同植物馆时为用户提供路径规划，优化市场上识别植物的功能。

### 核心价值
基于植物园游客游玩时想知道植物信息的需求，解决园区人流量过多时用户能及时获得植物信息的问题。

### 产品目标
* 拍下或上传植物照片，返回该动物该植物的名称及跳转相关百科信息。
* 输入植物园名，返回路径规划，帮助用户寻找园区。

### 目标用户
* 无法清楚得到植物信息的成人游客
* 想要了解更多知识的儿童群体游客
* 不熟悉植物园的游客


### 核心价值与用户痛点
#### 核心价值	
* 植物识别功能通过拍摄植物照片获取该植物的基础信息	
* 植物识别功能通过拍摄植物照片获取植物详细信息	
* 路线规划功能可以对从当前位置到植物园任一园区进行路线导航	

#### 用户痛点
* 植物原人流量过多，没有办法看到植物介绍栏
* 想给孩子普及植物知识，但对植物的了解有限
* 不熟悉植物园，不知道如何到达想要去的园区



### 需求列表与人工智能API加值
#### 需求列表

| 功能 | 用户案例 | 重要程度 |
| :------| ------: | :------: |
| 动物识别 | 用户想了解当前观赏植物的基础信息 | 重要 |
| 动物识别 | 用户想了解当前观赏植物详细信息 | 重要 |
| 路径规划 | 用户想知道当前位置到目标园区的路线 | 次重要 |
#### 具体应用场景
1. 小张在植物园观赏植物，此时他看到一种植物，想要植物的名称，但他孤身一人，且没找到植物简介的信息栏，于是他打开植物通，拍下植物照片上传，返回了植物的名称以及详细信息。
2. 周末妈妈带着儿女小兰到植物园游玩，但植物园人流量过多，许多游客站在信息栏前看植物简介。此时妈妈拿出手机打开了植物通app，让小兰拍下动物照片，获取了植物的百科信息
3. 小赵想去“樱花园”，但不熟悉植物园。这时小赵打开植物通，输入了“樱花园”，返回了当前位置到“樱花园”的路线导航。


#### 调用的API
* 百度AI动物识别
* 高德地图路径规划

### 人工智能概率性与用户痛点
#### 百度AI植物识别
* 支持识别超过2万种通用植物和近8千种花卉，接口返回植物的名称，并获取百科信息，适用于拍照识图类APP中
* 在拍摄和上传图片极为模糊时，识别植物信息不准确。
* 网络不佳，以及照片中存在人物或其他的情况下，无法识别植物。

#### 高德地图路径规划
* 此功能基于全面的路网信息和实时路况更新而精准率高，但位置太偏路网络信息未更新或者时GPS信号弱而影响使用。

### API调用
##### 百度植物识别API
1. API调用代码
![植物识别api调用代码](https://github.com/NFUNM172018125/API_ML_AI/blob/master/zhiwu1.png)
上传图片
![植物图片](https://github.com/NFUNM172018125/API_ML_AI/blob/master/songshu.jpg)
输出：植物名称、百科词条url、百科内容描述
![植物识别返回结果](https://github.com/NFUNM172018125/API_ML_AI/blob/master/zhiwu2.png)

