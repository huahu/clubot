## 安装配置
### 平台
python2.7
### 安装
```bash
pip install -r dev_requirements.txt
```

因少量的使用Linux shell命令,所以需要再win下运行需要对代码进行稍微的修改
### 配置
在settings.py填入bot的帐号和密码,和相应的管理员信息,关闭DEBUG
### 运行
```bash
python clubot.py      # 运行
```

## 更新内容
1. 使用`SQLAlchemy`重写数据库和逻辑部分
2. 清除不常用的命令
3. 将`history`命令改为`old`, 并对其增强
4. 将`mainloop`改为仙子的`tornado`MainLoop

## 更新到新版本
新版本对数据库做了较大的改动,  可以使用`update.py`脚本导入老数据

欢迎加入clubot@vim-cn.com讨论(gtalk 会出现丢消息的状况, jabber.org更是偶尔的不投递消息,甚至是两三天,所以换到vim-cn.com)

## 更新
### 2013-05-24
* 加入Python shell功能, 可以为每个成员分配一个session来保存语句上下文

### 2013-05-28
* 加入`HTTPStream`支持更快的HTTP请求
* 通过`HTTPStream`支持更快的Python shell
* 当Python shell返回过长时贴到网页上, 防止刷屏

### 2013-07-17
* 清除废弃的代码
* 改用HTTPStream废弃并清楚线程池
* 更新HTTPStream
* 废弃`-py`命令
* 废弃`-trans`命令, 使用`-tr`命令

### 2013-07-18
* 不使用 fork 将进程至于后台
* 不再解析命令行参数

### 2013-07-30
* 增加`TRACE`选项
