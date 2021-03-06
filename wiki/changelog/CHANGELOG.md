## v0.3.1
修复bug为主

* (修复) 数据库超时bug    @kid143

* (修复) web terminal支持复制粘贴   @liuzheng712

* (修复) 命令记录不准确bug    @kelianchun

* (修复) 连接断开提示Index out of ..bug    @kelianchun

* (整合) Tornado和Django框架，只需要启动一个端口    @liuzheng712

* (修复) 批量命令回车bug     @ibuler

* (修复) 日志审计中获取来源IP bug     @liuzheng712

* (修复) sudo 命令小写all 引起的推送失败(map)    @yumaojun03

* (修复) 定期处理在线用户的失效连接    @ibuler

* (修复) freebsd 推送带sudo规则的用户时 , sudo　路径引发的问题      @yumaojun03
 
* (修复) 进入系统内部 bug    @ibuler

* (修复) 特殊编码导致web terminal和录像挂掉bug    @liuzheng712 @kelianchun

* (修复) 禁用用户还可以登录跳板机bug    @ibuler

* (修复) “阻断”bug    @liuzheng712

* (修复) WebTerminal复制粘贴功能    @liuzheng712

* (更改) 文件上传路径和目录结构    @ibuler

* (更改) 启动脚本      @ibuler

* (更改) 配置文件

* (更改) 配置文件注明ws

* (更改) 通过jumpserver.conf来进行配置访问ip和端口   By @liuzheng712

* (更改) 用户下载私钥文件后删除   By @liuzheng712

* (更改) 强制用户使用key登录跳板机   By   @ibuler

* (更改) 统一一些文案   By   @ibuler

* (更改) 推送系统用户时，仅选择推送密钥时，不再推送key    By @yumaojun03
 
存在问题
* 取消了web terminal窗口大小改变功能，影响录像效果

* 之前的录像不再能观看

* 暂时还不支持windows

## v0.3.0
对核心代码进行了完整的重构

* (新增) 文件上传下载

* (新增) 主机搜索

* (新增) web terminal

* (新增) web端批量命令执行

* (新增) 录像回放

* (新增)  资产增加硬件信息抓取

* (新增) 资产增加Excel导出和导入

* (新增) 资产增加批量更改

* (新增) 添加系统用户推送

* (新增) 增加执行命令日志审计

* (新增) 增加文件上传命令审计

* (新增) 增加web端历史命令搜索

* (改进) 精确记录执行命令

* (改进) 优化脚本

* (改进) 授权细颗粒化

* (更改) 更改为输入ID登陆主机

* (更改) 执行命令使用ansible执行

* (更改) 废弃了LDAP支持，改为在主机上授权系统用户(系统用户为一些通用用户，如dev,dba等)

* (更改) 授权改为以授权规则为中心

* (更改) 更改sudo管理

* (更改) 取消权限申请

* (更改) 取消部门管理员

* (更改) 取消资产别名



## v0.2.0
对核心代码进行了完整的重构

* (新增) 使用别名或备注登录 

* (新增) 主机分组查看，使用更方便 

* (新增) 增加部门管理员负责管理本部门成员

* (新增) 增加仪表盘统计信息

* (新增) 增加部门， 用户组， 主机组 

* (新增) 主机登录方式增加登录方式 map，用于登录不支持ldap的主机 

* (新增) 增加主机批量修改，批量添加 

* (新增) 添加用户自动生成随机密码，然后自动发送邮件
 
* (新增) 添加各种搜索
 
* (新增) 增加普通用户web页面的授权申请

* (新增) 主机添加过滤搜索功能

* (新增) 增加用户头像
 
* (新增) 增加部门管理员页面

* (改进) 多线程批量执行命令
 
* (改进) 优化登录脚本

* (改进) Web界面更加美观漂亮

* (改进) 用户信息，主机信息更加详细
 
* (改进) 审计界面更加友好

* (改进) 上传批量上传 

* (改进) 普通用户页面内容更加丰富

* (更改) 主机授权，sudo授权改为组组之间授权
 
* (更改) 使用paramiko原生ssh协议登录后端主机(原来版本使用pexpect模拟登录）

## v0.1.1
对核心代码进行了完整的重构

* (新增) Web控制sudo

* (新增) Web查看统计日志

* (新增) Web实时查看session屏幕

* (新增) Web可以结束用户session

* (新增) 区分组管理员和超级管理员

* (新增) web上传和下载文件

* (新增) 批量执行命令记录日志

* (新增) 上传下载记录日志

* (新增) 用户可以web修改密码

* (新增) admin可以修改用户信息

* (新增) IDC

* (改进) 登录更稳定

* (改进) 支持分页

* (更改) 去掉shell脚本，来添加用户

* (更改) admin可以下载用户key


## v0.1.0
