## V2Manager(Beggar Version)
一个开源的使用Golang编写的V2Manager(适配V2raySocks)

# 当前版本
* Beggar - V0.1
* 本Manager使用的是Gold版的原生代码，不是那种各种Bug的捣糨糊产物
* 同步维护与Gold版Manager共有的代码部分
* 编译版只提供64bit版本，适用于64bit的所有linux系统(CentOS, Debian, etc)
* 欢迎关注频道 [V2Manager](https://t.me/V2Manager) 获取更新通知

# 使用方法
* ```./V2Manager```

# 实现的功能
* 连接Mysql的全套功能保留(Mysql连接语句已优化，连接池处理也全部保留)
* 用户处理的全套功能保留(增删用户，上传流量，关闭超量用户等)
* V2Ray异常关闭自启动
* 自定义Config和V2ray的Config路径(--cfg /home/config.json --v2cfg /home/v2ray.json)
* 完全开源，可自行编译修改。

# 如何开启更多V2Ray的功能
* 自行修改v2ray.json即可

# 阉割的功能
* 除了最基本后端应该具备功能的全部功能

# 完整版如何获取
* 对于喜欢更多自定义设置的高端用户，我们提供收费版的Manager供您玩耍。
* 收费版Manager包括更多的自定义设置，更多的自定义功能，以及状态回馈等
* 购买Manager [V2射线管理器开发组](https://t.me/V2rayIsNotGreat)

# 配置文件详解
名称 | 定义 | 示例值
:- | :- | :-
Mysql_Host | Mysql服务器地址 | 127.0.0.1
Mysql_Port | Mysql端口 | 3306
Mysql_User | Mysql用户 | root
Mysql_Password | Mysql连接密码 | 123456
Mysql_Db | V2ray用户数据所在数据库 | MyV2Ray
Mysql_TLS | 是否开启TLS/SSL | false, true, skip-verify
Mysql_MaxOpenConns | Mysql打开数据库的最大连接数 | 100
Mysql_MaxIdleConns | Mysql连接池中的最大保持连接数 | 10
V2rayClientAddr | V2Ray的api传入地址:端口 | 127.0.0.1:8301
V2rayTag | V2Ray的api标签 | proxy
Email | V2Ray用户邮箱后缀 | @123.moe
AlterID | V2Ray的用户额外ID | 64
Level | V2Ray的用户等级 | 1
CheckRate | 流量更新检查时间(秒) | 60

* Mysql_TLS 注意：true是开启，skip-verify是使用自签发或者无效的证书，false是不启用

# 其他
* 本项目没有任何隐藏后门和恶心人的Bug，我不喜欢干这事，担心乞丐版有什么问题自己审计代码自己编译。
* 本项目不包含任何授权系统，也不欢迎任何人添加授权系统。
* 本项目保留的部分和目前完整版代码是一样的，所以功能也是一样的，不需要担心体验差或者怎么样。
* 本项目遵循GPLV3，欢迎喜欢本项目的人参与编辑
* 有Bug请再ISSUE中提交完整的报错代码，我不是神仙解决不了没LOG的Bug

# 捐赠
* ETH钱包 0xaD8ABb15e4B8B58f5FbEE9CAb42096c1d640C234
* 链克钱包 0x4cfa7215324f2cc521beeb35c8a85c9afdbcda7e
* <a href='https://ko-fi.com/U7U7K54E' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi4.png?v=f' border='0' alt='Buy Me a Coffee' /></a>

# 更新日志
* 0.1.2 修正无上传/下载时的报错问题(V2ray 3.46)
* 0.1 代码删减完成，上传主体
