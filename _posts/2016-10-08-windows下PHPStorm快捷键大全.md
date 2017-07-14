---
layout: post
title: windows下phpstorm快捷键大全
description: 此快捷键说明我是翻译官方的快捷键说明的，方便查看，基于windows下PHPStorm的官方Help来翻译的，其中如有错误，欢迎斧正。
key: 程序员
---
## 说明 ##
此快捷键说明我是翻译官方的快捷键说明的，方便查看，基于windows下PHPStorm的官方Help来翻译的，其中如有错误，欢迎斧正。

## 编辑 ##
---

| 快捷键组合 | 说明 |
|---|---|
| Ctrl + Space | 代码自动完成提示（选择） |
|Alt + Enter | 显示意图动作和快速修复 |
|  Ctrl + P | 参数信息（在调用方法参数忘记的时候，提示）|
| Ctrl + Q | 快速查找文件，可以查找当前类定义的文件等 |
| Ctrl + 鼠标滑过 | 基本信息 |
| Alt + Insert | 生成代码...(细节需要多次操作会发现很有意思)|
| Ctrl + O | 重写方法（在PHPStorm中是重写父类方法，会有选择框） |
|Ctrl + I | 实现方法（一般是指实现接口类或抽象类方法） |
|Ctrl + Alt + T | 环绕代码块 (if..else, try..catch, for, 等) |
|Ctrl + / | 单行注释(//) |
|Ctrl + Shift + / | 块注释 (/**/) |
|Ctrl + W | 选择依次递增的代码块，具体使用目前来看比较少 |
|Ctrl + Shift + W | 去掉当前选择返回上一个选择，类似于撤销选择，与上面的相反 |
|Ctrl + Alt + L | 格式化代码，一般来说，写的代码格式不整齐统一，这个很有用 |
|Ctrl + Alt + I | 自啮合线，这个解释不太好解释，测试结果就是会自动根据代码来进行对齐 |
|Ctrl + D | 复制当前行或选定的块 |
|Ctrl + Y | 删除插入符号所在行 |
|Ctrl + Shift + J | 智能线连接（HTML和JavaScript才有用） |
|Ctrl + Enter | 智能分割线 (HTML 和 JavaScript 才有用)  |
|Shift + Enter | 开始新行，比如光标在当前行，不需要切换到行尾按Enter，直接按这个组合键即可 |
|Ctrl + Shift + U | 切换选中的英文文字的大小写，此处其实用到挺多的 |
|Ctrl + Shift + ] 或 [  |  选择直到代码块的开始或结束，我之前不知道这个，其实很有用 |
|Ctrl + Delete | 删除从当前光标到当前单词结尾 |
|Ctrl + Backspace | 从光标位置删除到当前单词的开始 |
|Ctrl + + 或 - | 这里是ctrl和加号或者减号产生的组合，可以折叠或展开当前代码块 |
|Ctrl + F4 | 关闭活动中的tab |
|Ctrl + Shift + V |  从历史粘贴 |

## 调试 ##
---
*此处我是用得很少*

| 快捷键组合 | 说明 |
|---|---|
| F8 | 跳过 |
| F7 | 步进 |
| Shift + F8| 跳出 |
| Alt + F8 | 表达式求值 |
| F9 | 恢复程序 |
| Ctrl + F8 | 切断断点 |
| Ctrl+Shift+F8 | 查看断点 |

## 运行 ##
---

| 快捷键组合 | 说明 |
|---|---|
|Shift + F10 | 运行 |
|Shift + F9 | 调试 |
|Ctrl + Shift + F10 | 从编辑器运行上下文配置（Run context configuration from editor），此处可能翻译不够准确 |
|Ctrl + Shift + X | 在命令行运行 |

## 搜索/替换 ##

| 快捷键组合 | 说明 |
|---|---|
| Ctrl + F/R | 查找/替换 |
| F3/Shift + F3 | 查找下一个/上一个 |
| Ctrl + Shift + F/R | 在目录中查找/替换 |

## 查找哪些地方使用 ##

| 快捷键组合 | 说明 |
|---|---|
| Alt + F7 / Ctrl + F7| 当前文件查找被使用/在文件中查找哪些地方使用 |
| Ctrl + Shift + F7 | 文件中搜索并在使用的地方高亮显示 |
| Ctrl + Alt + F7 | 显示哪些地方被使用 |


## 导航 ##
---
| 快捷键组合 | 说明 |
|---|---|
|Ctrl + N | 跳转到指定类 |
| Ctrl + Shift + N | 跳转到文件 |
| Ctrl + Alt + Shift + N | 跳转到符号|
| Ctrl + G | 跳转到第几行 |
| Alt + Right/Left | 切换编辑器活动窗 |
| Esc | Go to editor (from tool window)|
| Ctrl + E | 弹出最近编辑文件，我也是在写这文档才知道，太方便了 |
| Ctrl + Alt + Left/Right | 导航前进/后退 |
| Ctrl + Shift + Backspace | 跳转到最近编辑的代码位置 |
| Alt + F1 | 在任何视图中选择当前文件或符号 |
| Ctrl + B 或 Ctrl + Click | 跳到申明（如跳转到当前函数声明的地方，这个很常用，可以实操一下） |
| Ctrl + Alt + B | 与上面相反，跳到执行位置 |
| Ctrl + Shift + I | 打开快速定义查找 |
| Ctrl + Shift + B | 跳转到类型声明 |
| Ctrl + U | 跳到超级方法(super-method)/超类 (super-class)|
| Alt + Up/Down | 跳转到上一个或者下一个方法，在编辑一个类的时候，方便一个一个的方法进行查看 |
| Ctrl + ] / [ | 跳转到代码块的开始或结束 |
| F2 / Shift + F2 | 跳转到上一个或下一个高亮错误地方，这个检查代码语法错误很有用 |
| F4 / Ctrl + Enter | 编辑源代码/查看源代码 |


## 重构 ##
---

| 快捷键组合 | 说明 |
|---|---|
| F5/F6 | 复制/移动 |
| Alt + Delete | 安全删除 |
| Shift + F6 | 重命名 | 
| Ctrl + Alt + N  | 内联变量 |
| Ctrl + Alt + M/V/F/C | 提取方法/变量/字段/常数(Method/Variable/Field/Constant) |
| Ctrl + Alt + Shift + T | 重构这段代码（显示所有可用的重构），比如if else if 这种语句转switch语句|


## VCS/本地历史  ##
---

| 快捷键组合 | 说明 |
|---|---|
| Alt + 反引号 (`) | ‘VCS’ 快速弹出，此处需要注意这个反引号在最左上角，和那个~符号在一起的，ESC键下面 |
| Ctrl + K | 提交项目到VCS |
| Ctrl + T | 从 VCS 更新项目 | 
| Alt + Shift + C | 显示最近更改 |


## 常用操作 ##
---

| 快捷键组合 | 说明 |
|---|---|
| 快速按两次 Shift  | 搜索任何一个地方 |
| Ctrl + Shift + A | 查找方法(Action) |
| Alt + #[0-9] | 打开相应的工具窗口（这个我也没搞明白） |
| Ctrl + Alt + F11 | 开启或关闭全屏模式 |
| Ctrl + Shift + F12 | 开启或关闭最大化编辑 |
| Alt + Shift + F | 添加到收藏列表（我觉得这个功能很神奇，不知道为啥要这么做） |
| Alt + Shift + I | 检查当前文件以及当前配置文件 |
| Ctrl + Alt + S | 打开设置对话框（表示会与QQ默认快捷键冲突） |
| Ctrl + Tab | 在 tabs 和工具窗口间切换 |


## 插入模板/片段(针对PHPstorm) ##
---

| 快捷键组合 | 说明 |
|---|---|
| Alt + J | 插入模板 |
| eco |  ‘echo’ 语句 |
| fore | foreach(iterable_expr as $value) {…} |
| forek |  foreach(iterable_expr as $key => $value) {…} |
| inc/inco |  ‘include’/‘include_once’ 语句 |
| prif  | private function |
| prof  | protected function |
| pubf | public function |
| rqr/rqro |  ‘require’/‘require_once’ 语句 |
|更多...| 其他自己尝试 |