
# Chatstack

Chatstack是一个全流程搭建中文NLU的用户交互系统。

有了Chatstack，用户不用写一行代码就能够搭建定制化的中文NLU模组：定义意图和实体、标注数据、训练NLU模型、管理模型、测试和部署NLU模组。

Chatstack后端特别为中文语言进行大量的机器学习算法优化，意图和实体识别准确率高、拓展性强，对训练数据的数量也没有太高的要求。

Chatstack同时拥有企业级的用户管理权限，管理员可以自主为其他用户添加或删除训练NLU、修改意图及实体设置、调整NLU版本设置及修改训练数据的不同权限。




### 意图管理

![](http://www.crownpku.com/images/201908/intent.png)

### 实体管理

![](http://www.crownpku.com/images/201908/entity.png)

### 数据标注

![](http://www.crownpku.com/images/201908/label.png)

### NLU模型管理

![](http://www.crownpku.com/images/201908/model.png)

### 账号管理

![](http://www.crownpku.com/images/201908/account.png)

### 部署NLU模型

在UI中选择生产环境之后，可以通过下面的https API调用生产模型：


```
curl -XPOST https://chatstack.crownpku.com:9091/model/parse?token=xxx -d '{"text":"我想请下个月3号到6号的假"}' | python -mjson.tool
```

我们设置了API token来防止恶意调取API。如有兴趣测试生产模型的API集成或加入微信讨论群，请联系“**Chatstack小助手**”微信号：**chatstack_cn**



### 公测demo在[chatstack.crownpku.com](http://chatstack.crownpku.com)

我们已经部署和开放了一套公测demo系统，供感兴趣的朋友免费试用。

关注微信公众号“**王耳古**”，回复"**chatstack**"获取公测用户名和密码。

感谢谷歌云赞助GCP credit supported activity.

### 文档在[https://github.com/crownpku/Chatstack-Doc](https://github.com/crownpku/Chatstack-Doc)

欢迎在上述github文档的Issues中提bug或建议新功能。


