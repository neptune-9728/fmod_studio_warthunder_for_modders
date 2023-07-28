#  来自官方库的副本 以后大更新可能会导致副本出错 建议使用官方库 副本只作参考!
## 官方库地址:https://github.com/GaijinEntertainment/fmod_studio_warthunder_for_modders

---

## 你需要注意的
请使用**2.1.6**版本的FMOD 过高会Build错误!
音频尽量使用**WAV**格式
---

# 我个人理解的教程
---

## 基于官方库创作:
1. 拷贝官方库到本地
1.1 关于库的内容 (你大概会用上的)
    **本地文件**  Assets -> **原声** Metadata -> **事件**

    dialogs_wt_tanks_2023 -> **新版本陆战乘员组语音包** （只有英配和俄配）
    radio_chat -> **空战无线电** 
    gui -> **部分UI音效**
    dialogs_wopl\english\voice_messages -> **无线电**

2.启动FMOD
2.1 关于FMOD的内容
    dialogs_crew_ground -> **乘员组**
    dialogs_crew_aircraft -> **无线电**
    airfraft\music -> **音乐**

3.导入的两种方法 B方法也是基于我的副本使用的导入方法
（A）直接将语音文件拖入事件中
（B）修改Banks路径到我想修改的语音文件夹中 具体操作:
举例修改中文客户端的陆战乘员组
    进入**Banks** 
    选择路径: dialogs_wt_tanks_new {_crew_dialogs_ground_new_zh -> Audio Table}
    点击Browse后选择存放要修改的语音包文件夹
    为要修改的语音事件创建**Programmer Instrument** 重命名和语音包文件夹要修改的语音文件一样的名字

4.导出
举例导出中文客户端的陆战乘员组 
    进入**Banks**
    选择路径: dialogs_wt_tanks_new {_crew_dialogs_ground_new_zh} + **{_crew_dialogs_ground_new}** 必要
    右键**Build**

5.使用
在完成导出的步骤后，进入本地库的文件夹
    进入路径 **Build** 会发现文件以及被生成好了
    将除了**masterbank**那三个文件 剩下的导入游戏**mod**文件夹内即可
---
## 基于我的副本修改:
其实和官方库没什么区别 还是建议使用官方库

+主要修改是给语音事件标注了颜色
    [绿色]单独使用的声音事件
    [红色]没有任何声音事件
    [在当前文件夹别的颜色]有重复或跨文件夹使用的声音事件
+移除了噪音事件
会导致生成的**masterbank**文件不能正常使用

## 更详细的教程或者我想说的会以后更新 因为现在涅涅子要睡觉了 XD