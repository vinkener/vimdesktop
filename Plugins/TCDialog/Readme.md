﻿## 帮助

### 可用命令
* `<TC_OpenTCDialog>`：打开 TC 进行文件选择，默认绑定到 `Win + o`

### 快捷键
* `Win + o`：在文件对话框或任意文字编辑界面按下快捷键跳转至 TC，再次按下快捷键选择当前文件（或已选文件）返回调用者
* `Esc`：离开 TC，回到调用者
* `Shift + 回车`： 当前目录返回调用者（一般用于保存文件）

## 更新历史

```
2020-06-03 @陌辞寒
--------------------------
去除自动跳转功能，简化按键绑定。因为之前用法复杂、容易出问题，我几乎不用。现在改简单些，可以会用一用。

2016-04-14 @杜立涛
--------------------------
优化将当前目录返回调用方的实现方法：方便保存文件时改名
修正路径名过长时，选定文件的字符串被截断的问题：
 * 第一步：粘贴文件夹路径，回车
 * 第二部：粘贴不带路径的文件名，回车

2016-02-23 @陌辞寒
--------------------------
不再新增 select 模式，改为重新映射快捷键，返回调用方前再清除快捷键，绕过 normal 模式下快捷键依然有效的 bug
支持将当前目录返回调用方（用于保存文件对话框）

2014-08-08 @杜立涛
--------------------------
跳过对标题栏为空的文件选择对话框——如 Eclipse 的已打开文件的列表

2014-03-12 @杜立涛
--------------------------
初步实现，并增加帮助说明
```
