## 功能：
##### 定时同步大佬的代码并触发部署到腾讯云函数；
##### 每天同步并部署2次，只有定时任务才可以触发部署，手动同步代码不会触发部署;
## 注意事项：
####1.main.yml文件所在分支要设置为默认分支，并且不能为master分支，我用的是main分支；（master用来放lxk0301大佬的代码的）
####2.要禁用`sync-lxk0301-scripts`这个workflow，效果如下图:
![img_1.png](icon/img_1.png)

### 使用到的环境变量：
| Name                          |   归属                  | 属性        |
| :---------------------:       | :----------:           | --------- | 
| `PAT`                         |Personal access token   | 必须 | 
| `DEPLOY_TG_BOT_TOKEN`         |telegram推送             | 非必须 |
| `DEPLOY_TG_USER_ID`           |telegram推送             | 非必须 |
| `DEPLOY_PUSH_KEY`             |微信server酱推送          | 非必须 |
| `editIndexJsFile`             |是否编辑index.js文件(填 true/false)      | 非必须 | 
