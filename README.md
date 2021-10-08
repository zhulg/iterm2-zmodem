# iterm2-zmodem
备份iterm2-zmodem的依赖脚本,用于MAC在云服务器上上传和下载文件，rz和sz进行上传和下载，可以用于包含跳板机的机器。

## 配置
- 打开一个iTerm终端，点击菜单的Profiles，选择某个profile之后然后继续选择advanced → triggers，添加triggers。
- 对应配置2个 

```
Regular expression：\*\*B0100
Action:  Run Silent Coprocess  
Parameters: /usr/local/bin/iterm2-send-zmodem.sh

Regular expression：\*\*B00000000000000	
Action: Run Silent Coprocess	
Parameters: /usr/local/bin/iterm2-recv-zmodem.sh
```
