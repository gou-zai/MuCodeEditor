# MuCodeEditor

### 最后更新于：2022/5/30 - 15:10

### 开源组 QQ 群：1032012046

## 一款流畅的大文本编辑器

免费且开源，你还在等什么！

## 协议

我们使用 MPL 2.0 作为开源协议，其中明确规定你可以拿来商用与修改，但版权永远属于本人（SuMuCheng）

除非我允许的情况下你不得做出侵权行为

## 功能：

基础文本编辑、文本选中、按可见行绘制（至少支持到 150w 行代码编辑）

行号显示

代码高亮：默认的 DefaultLexCoroutine 实现了 LexCoroutineInterface，使用协程（Coroutine）实现 Lexer 异步分析

不会影响主线程，即在 I/O Coroutine 中进行 span 操作

打开文件 & 保存文件 的支持

## 样式

你可以自定义样式，对于统一的操作我们使用 Controller

例如自定义主题你只需要继承 AbstractTheme 以实现自己的主题，再在 Controller 中修改即可

目前已实现：

光标移动动画

## 扩展性

我们对于很多组件设置了 open 而不是 finally ，你可以继承它们以实现自己的功能

## 封装性

我们对于很多组件进行了封装，例如 Lexer 中的 isLetter，isDigit，isWhitespace ...

都在 BaseLexer 中定义

## 后续

增加 Parser 以实现更深层次的语法解析和自动补全

增加 Redo & Undo 以实现撤销和回退

增加 ToolOptionsPanel 实现快捷全选、复制、粘贴

增加 CursorFlickerEffect 实现光标闪烁

# 部分思路来源于 Rosemoe's Editor
https:// rosemoe.github.io/2020/02/15/highlight-editor-creation/

## 以下是使用截图

<img src="./pictures/example1.jpg" width="40%" height="auto"></img>

<img src="./pictures/example2.jpg" width="40%" height="auto"></img>