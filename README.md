# TG群 https://t.me/InteIJ 前期脚本经常修复，建议加群(仅个人建议)

#### 根据变量运行自动运行对应任务
## 爬虫源码仓库 https://github.com/XgzK/TGreptile
本项目主要为国内没外网环境的人准备的公益项目

## 特别声明

```text
有问题可以 https://t.me/InteIJ 群组联系
需要其他功能的可以反馈添加，或者反馈脚本BUG问题
有如果有其他获取参数的可以反馈给我添加
本项目所有活动来自TG各大频道,本项目偷免单助力介意勿用
害怕偷CK的勿用,不接受任何形式甩锅,不对任何行为负责
```


### 容器构建命令
```shell
docker run -dit \
  -p 自定义:5008 \
  -e TZ=Asia/Shanghai \
  --name qlva \
  --restart unless-stopped \
  xgzk/qlvariable:latest
```
```http request
http://IP:自定义端口/ 提交和更新页面
http://IP:自定义端口/log 日志页面
```
需要定时任务配置文件权限

### amd64拉取容器可能报错
在拉取时候添加
```shell
--platform linux/amd64
```
```text
standard_init_linux.go:219: exec user process caused: exec format error
```
## 更新说明

```text
版本1.1 
 > 修复不同版本数据库差异问题
 > 添加去重功能
 > BUG未知，请遇到反馈
版本1.1.1
    > 修复重复提示不清楚问题
    > 增加请求次数，由原来一次请求失败，现在可以最多请求三次，只要成功一次，就不再请求了
    > 优化活动参数重复提醒
版本1.1.2
    > 适配了特别10.2版本，把10.2之前包括10.2定义为9版本
版本1.2
    > 更新可以保留conn.yml文件
    > 对一些获取进行不去重处理
    > 建议之前版本拉取最新脚本
版本1.3
    > 添加了配置文件检测
    > 修补了缺少的文件
    > 添加了10版本以上数据库表的检测
版本2
    > 正式启用容器版本
    > 取消了复杂的配置,改用程序自动适配
    > 有了自动更新省去了更新繁琐的步骤
```
