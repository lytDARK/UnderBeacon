# 命令存储（command_storage）
假设命名空间为`x`：

临时存储：使用`cache:x`，
1. 如果是瞬间读取可以使用`cache:cache cache`。对于这种空间的利用要先初始化

配置：使用`x.config:y`。
1. 主要内容可以用`x.config:data`，
   1. 如版本信息可以用`x.config:data version`
2. 玩家数据可以用`x.config:playerdata`等。

配置导出：可以使用`config.x:y`，
1. 主要内容可以用`config.x:data`，
   1. 版本信息更建议用`x.config:data dataversion`，毕竟是导出信息嘛~
2. 玩家数据可以用`config.x:playerdata`等。
3. 当然如果有用户界面等会更好啦~