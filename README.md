# dingtalk sso
钉钉免登接口，ISV套件和企业号通用。

##安装 
`npm install dingtalk_sso`
##示例
构造函数：
```js
var dingtalk_sso = require('dingtalk_sso');
var conf = {
    corpid: 'dingxxxxxxxxxxxxxxx',
    SSOSecret:'C1oXyeJUgH_QXEHYJS4-Um-zxfxxxxxxxxxxxxxxxxxx-6np3fXskv5dGs'
  }
var api = new dingtalk_sso(conf);
```
##方法
### 通过CODE(免登授权码)换取用户身份
```js
api.getSSOUserInfoByCode(code, callback)
```
### 生成授权链接
```js
api.generateAuthUrl(redirect_url)
```
##更多钉钉相关
ISV套件主动调用API: [dingtalk_suite](https://github.com/hezedu/dingtalk_suite)<br>
ISV套件回调serverAPI: [dingtalk_suite_callback](https://github.com/hezedu/dingtalk_suite_callback)<br>
企业号API: [dingtalk_enterprise](https://github.com/hezedu/dingtalk_enterprise)
