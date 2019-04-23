# ET-RPG-DEMO
仅供学习交流.  
目标是在ET框架的基础上,做一个支持多人对战的ARPG的DEMO.   
借以学习服务器端开发.和了解服务器/客户端交互细节.  

## 项目特点   
1.同步方式为状态同步(似乎有点像混合同步? 反正刚接触服务器开发,不太了解这块的区别)   
2.双端物理(BOX2D,模拟3D)  
3.ARPG,支持多人对战

# 目前目标和进度的说明   
## 已完成
1.导入一套动作资源,创建基本Animator     
2.创建一套UI框架,规范UI这边的工作流    
3.实现简单的移动同步(目前是一秒同步5次)    
4.初步实现了服务器/客户端 逻辑帧框架,以及完善了移动同步    
5.移动同步更改为45度俯视角   
6.双端移动&使用技能已经完成同步.

## 进行中   
6.重构BUFF系统,调整服务器这边下发技能命中后的效果播放消息的处理.
7.加入双端行为树,制作支持多人合作的副本

## 进度展示(视频连接,占位)


## 注意事项
1.技能系统目前只同步了使用方向的.需要锁定目标和指定位置的技能使用的同步请自行仿照相关代码添加对应的协议和逻辑代码.(UnitStateComponentSystem)   
2.BattleTest场景为客户端这边搭建的单机测试场景.    
3.Server端这边请打开sln工程后直接重新编译,再运行. 目前其他方式打开服务器有点问题.我暂时没时间去解决.
4.有些代码写的很挫,觉得太low的可以跟我提一下,我修改修改. :)

## 技能系统设计思想
https://blog.csdn.net/qq_32270109/article/details/88551196




