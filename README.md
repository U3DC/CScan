# CScan：一键快速打印项目代码行数

## 引言
你当前项目的代码量是多少？<br>
你的模块一共写了多少行代码？<br>
如果去掉注释和空白行你的代码量又是多少？<br><br>

想知道这些问题吗，那么就快使用CScan吧！<br>


## 用途
帮助开发者了解当前项目的代码体量。<br>


## 如何使用
1、将代码clone或解压到Assets/下的任何目录；<br>
2、在"Project"窗口选中需要扫描的文件或文件夹（支持多选）；<br>
3、在菜单栏选择"CScan"，根据需求选择输出模式：<br>
	* All //所有行<br>
	* Ignore Invalid //忽略空白行、注释<br>

## 原理及相关定义
通过Selection获取选中的文件，通过正则统计。<br>

无效行过滤思路<br>
1. 去除头尾空行；<br>
2. 将所有行注释替换为空；<br>
3. 将所有块注释替换为空；<br>
4. 缩进无效换行。<br>



