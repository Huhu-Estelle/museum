## 智能博物馆PRD
### 价值主张
提供便利的展品查找服务，当用户在网上看到馆内展品图时，应用事先采集展品照片并标记分组，为图像识别技术提供信息素材。不需要在收索引擎对图片进行文字描述，也不需要苦苦等待照片发布者的回复，只需要上传展品图片，应用自动返回相应的展品、展馆介绍。根据通用物体和场景识别API自动返回相应的展品、展品介绍以及通过危险行为识别API对展品有一个基础的保护措施。APP也会记录、分析用户上传的图像，不断提高识图准确性。
### 产品概述
用户在应用上传展品或者地标图片，通过图像识别返回展品的基本信息及对展品起基础保护作用。
### 加值宣言
- 1.（核心）[通用物体和场景识别API](https://ai.baidu.com/tech/imagerecognition/general)： 当用户在社交平台上看到他人分享的馆内展品图，并对此感兴趣想要进一步了解时，不需要在收索引擎对图片进行文字描述，也不需要苦苦等待照片发布者的回复，只需要上传展品图片，应用自动返回相应的展品、展馆介绍，快速方便。 图像识别api设置定制化识图，通过图片内容识别给图片打上标签，检索与标签相关的信息，适用于图像搜索等场景。
- 2.（辅助）[百度人体检测与属性识别API](https://ai.baidu.com/tech/body/attr)： 根据监控录像识别可能患有多动症的儿童，自动追踪，当目标人的举动有可能导致展品破损时，向周围管理人员发送通知，让管理员多加注意，降低展品破坏事故的发生几率。 人体检测与属性识别api可以检测图像中所有人体，识别20余类属性信息，包含性别年龄、服饰佩戴、行为动作等。
### 核心价值
用户上传展品或者展馆图片，通过图像识别返回展品的基本信息及展品起基础保护作用。
### 用户痛点
- 1.当用户在社交平台上看到他人分享的馆内展品图，并对此感兴趣想要进一步了解时，不想直接询问图片发布者，也不知如何搜索、描述图片。
- 2.身障者不便穿过人群靠近阅览展品介绍。
- 3.多动症儿童容易不小心破坏展品，监护人谨慎看管孩子时难以集中观赏展品。
### AI概率性考量
#### 需求列表与人工智能API加值
| 使用场景 | 用户需求 | 重要性 | 技术
| ------ | ------ | ------ | ------ |
| 用户在社交平台上看到他人分享的馆内展品图或在观览时不便穿过人群靠近阅览展品介绍| 识别照片中的展品反馈简介 | 非常重要 | 通用物体和场景识别API
| 多动症儿童容易不小心破坏展品，监护人谨慎看管孩子时难以集中观赏展品 | 安保人员协助看管 | 重要 | 百度人体检测与属性识别API
## 原型
[产品原型](http://nfunm022.gitee.io/museum_app)
### 拍照模块（搜索展品信息及展品摆放位置）
![image](https://github.com/Huhu-Estelle/museum/blob/master/%E6%8B%8D%E7%85%A7.png)
##### 用户使用拍照把图片通过通用物体和场景识别API，给图片打上标签，检索与标签相关的信息，并告诉用户展品在展馆的所处位置。
### 我模块（快速查找收藏展品）
![image](https://github.com/Huhu-Estelle/museum/blob/master/%E6%88%91%E7%9A%84.png)
### 用户可以通过收藏快速找到感兴趣的展品，查看相关信息。
