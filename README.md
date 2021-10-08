# iterm2-zmodem
iterm2-zmodem的依赖脚本

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