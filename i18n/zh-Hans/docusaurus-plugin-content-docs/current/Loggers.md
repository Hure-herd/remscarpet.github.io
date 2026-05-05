# 记录器

## 地狱门POI
`/log displaypoi`  
通过在poi上渲染一个紫色玻璃来显示POI  
![log_displaypoi-1](/img/loggers/log_displaypoi-1.png)
![log_displaypoi-2](/img/loggers/log_displaypoi-2.png)

左图为未开启状态，右图为开启状态

属性:
- 默认选项: N/A
- 参考选项: N/A

## 查看区块加载情况
`/log loadedChunks`  
一个 HUD 记录器
显示整个游戏世界里指定/全部维度的区块加载情况  
![log_displaypoi-2](/img/loggers/log_loadChunks-zh.png)

从左到右分别是:`全部世界`,`主世界`,`地狱`,`末地`  
左侧数字代表强加载区块数量，右侧数字代表弱加载加上强加载的区块总数

属性:
- 默认选项: `brief`
- 参考选项: `brief`, `overworld`, `nether`, `end`, `full`