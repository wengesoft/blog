下面是bat文件测试代码
```batch
@echo off&@setlocal EnableDelayedExpansion
title 字体属性控制码测试
rem 字体前景色
set forecolor=黑色 红色 绿色 黄色 蓝色 紫色 天蓝色 亮白色
set ct=30
for %%a in (%forecolor%) do (
   echo [1;!ct!m%%a
   set /a ct+=1
)
echo [4m下划线
set /p=[0m清除属性
```
只是选用了一些实用的ANSI控制码，更多功能控制码转参考文献。
