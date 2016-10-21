# Sublime Text 3 功能、配置及插件

*访问 [packagecontrol.io](https://packagecontrol.io) ，可下载插件、主题及配色。*

## Features（功能）

**Command Palette （命令面板） `command + shift + p`**

命令面板可以使你访问设置菜单中可以所有的东西，调用包命令，更改文件的语法，处理Sublime项目，等等。举例来说，你可以在命令面板中Git命令添加，分支，提交和推送。


**File Switching （文件切换） `command + p`**

Sublime Text提供了一个非常快速的方式来打开新的文件。只要按下command+ P并开始输入你想要打开的文件的名称。一旦找到文件，只需按enter键，就可以开始直接输入到该文件了！

**Goto Symbols （跳转标记） `command + r`**

当你编辑一个大文件时，文件中有一堆方法，按command + R将其全部列出来，使他们更容易找到。开始尝试的输入你想要的，然后按Enter 就可以快速跳转这个方法了。
Sublime Text 3 有一个新功能（Goto Definition 转到定义）。它提供了 Sublime Text 更多功能，使其更接近于一个IDE。如果你有兴趣，可以自己去学习一下。

**Multi-Edit（多行编辑） `command + click`**

有许多不同的方式使用多行编辑：

- `command + d`: 选中光标所占的文本，继续操作则会选中下一个相同的文本。
- `command + l` 选中整行，继续操作则继续选择下一行，效果和 shift+↓ 效果一样。
- `command + shift + l` 先选中多行，再按下快捷键，会在每行行尾插入光标，即可同时编辑这些行。
- `option + 鼠标向上拖动` 或 `command + option + 鼠标向上拖动` 向上添加多行光标，可同时编辑多行。
- `option + 鼠标向下拖动` 或 `command + option + 鼠标向下拖动` 向下添加多行光标，可同时编辑多行。
- `shift + ↑` 向上选中多行。
- `shift + ↓` 向下选中多行。

**Snippets（代码片段）**

代码片段是Sublime Text的另一大特点。您可以使用预装的，也可以自己创建，或安装具有代码片段的包。你所要做的就是输入一个定义了代码片段的文本，它会扩展到你的代码段。
例如，键入lorem将产生lorem存有文本。
使用: 输入一个定义了代码片段的文本（例如lorem），然后按tab键。

[http://www.hongkiat.com/blog/sublime-code-snippets/](http://www.hongkiat.com/blog/sublime-code-snippets/)

**Keyboard Shortcuts （快捷键）**

Sublime Text的快捷键的数量是惊人的。我觉得这是Sublime Text另一个好的功能。如果太多了，你可以将自己常用的快捷键从主键（ home keys ）移到了自己的快捷键列表中（my keyboard）。
对于Sublime Text键盘快捷键的完整列表，看看我们的键盘快捷键文章。[https://scotch.io/bar-talk/sublime-text-keyboard-shortcuts](https://scotch.io/bar-talk/sublime-text-keyboard-shortcuts)

**Projects（项目）**

在Sublime Text中，项目是工作流程中不可或缺的一部分。一个项目仅仅是一个 Sublime工作空间，项目中的文件夹都是开放的，并显示在侧边栏中。这是很有帮助的，因为你可以定义一个项目，并添加文件夹到项目中，并能够迅速地在文件夹之间切换。
使用项目，你只需要去Finder中找到你想要的项目，并将其拖到Sublime Text，就可以了。

保存一个项目：进入命令面板，输入保存项目。

切换项目：command + control + p

## Settings（设置）

Sublime自带了大量的设置。我建议你去看看它所提供的所有设置。

为了让您进入用户设置，使用命令面板并且键入user。
这里是我当前的设置。

```json
{
	"always_show_minimap_viewport": true,
	"bold_folder_labels": true,
	"build_systems":
	[
		{
			"name": "List",
			"shell_cmd": "ls -l"
		}
	],
	"caret_extra_bottom": 1,
	"caret_extra_top": 1,
	"caret_extra_width": 1,
	"caret_style": "smooth",
	"color_scheme": "Packages/User/SublimeLinter/base16-summerfruit.dark (SL).tmTheme",
	"font_face": "Monaco",
	"font_size": 15,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"ignored_packages":
	[
	],
	"indent_guide_options":
	[
		"draw_normal",
		"draw_active"
	],
	"line_padding_bottom": 2,
	"line_padding_top": 2,
	"overlay_scroll_bars": "enabled",
	"save_on_focus_lost": true,
	"scroll_past_end": true,
	"scroll_speed": 1.0,
	"show_line_endings": true,
	"tab_size": 2,
	"theme": "Boxy Tomorrow.sublime-theme",
	"theme_accent_green": true,
	"theme_find_panel_size_xs": true,
	"theme_icon_button_highlighted": true,
	"theme_scrollbar_colored": true,
	"theme_statusbar_size_xs": true,
	"theme_tab_arrows_hidden": true,
	"theme_tab_selected_filled": true,
	"theme_tab_separator": true,
	"translate_tabs_to_spaces": true,
	"trim_automatic_white_space": true,
	"trim_trailing_white_space_on_save": true,
	"wide_caret": true,
	"word_wrap": true
}

```
下面是另一份简单配置：


```json
// User/Preferences.sublime-settings
{
  "bold_folder_labels": true,
  "color_scheme": "Packages/Theme - Flatland/Flatland Monokai.tmTheme",
  "font_face": "Ubuntu Mono",
  "font_options": "subpixel_antialias",
  "font_size": 14,
  "highlight_line": true,
  "highlight_modified_tabs": true,
  "ignored_packages":
    [
    ],
  "line_padding_bottom": 1,
  "line_padding_top": 1,
  "rulers":
    [
      80
    ],
  "scroll_past_end": true,
  "tab_size": 4,
  "tab_completion": false,
  "theme": "Soda Light.sublime-theme",
  "translate_tabs_to_spaces": true,
  "trim_trailing_white_space_on_save": true,
  "vintage_start_in_command_mode": true,
  "word_wrap": true
}
```

我在Sublime中用的是最佳模式。它提供了 vi 编辑命令代替Sublime Text。它不是原vi包的全功能，但它是我目前见过最接近 vi编辑器的文本编辑器。使用你的键盘快捷键和命令包就可以非常快速的开发。
上面的设置会在你打开一个文件时自动开启Vintage模式（注：Vintage是Sublime Text的vi模式编辑包。可以使用组合vi命令来调用Sublime Text的功能，包括多重选择。）。
如果你不喜欢这个功能，只是删除vintage_start_in_command_mode就可以了，如果你想完全禁用Vintage模式，那么删除ignored_packages设置。

## Packages/Plugins（包/插件）

**Package Control（包控制）**

Sublime Text提供了绝对必要的包管理器。这是安装下面列出的所有插件和主题的最佳方式。继续，在包控制在安装插件。
使用方法：进入命令面板（command + shift+ p），然后键入 install。

个人推荐：**[Better CoffeeScript](https://packagecontrol.io/packages/Better%20CoffeeScript)** **[Better JavaScript](https://packagecontrol.io/packages/Better%20JavaScript)** **[BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter)** **[Clickable URLs](https://packagecontrol.io/packages/Clickable%20URLs)** **[Color Highlighter](https://packagecontrol.io/packages/Color%20Highlighter)** **[DashDoc](https://packagecontrol.io/packages/DashDoc)** **[DocBlockr](https://packagecontrol.io/packages/DocBlockr)** **[Emmet](https://packagecontrol.io/packages/Emmet)** **[FileDiffs](https://packagecontrol.io/packages/FileDiffs)** **[Javascript Beautify](https://packagecontrol.io/packages/Javascript%20Beautify)** **[Pretty JSON](https://packagecontrol.io/packages/Pretty%20JSON)** **[Themr](https://packagecontrol.io/packages/Themr)** **[Trimmer](https://packagecontrol.io/packages/Trimmer)** **[Web Inspector](https://packagecontrol.io/packages/Web%20Inspector)** **[Terminal](https://packagecontrol.io/packages/Terminal)** **[SublimeCodeIntel](https://packagecontrol.io/packages/SublimeCodeIntel)**

**Alignment （代码对齐）**

一个非常简单和易于使用的插件,使你的代码组织和美观。当您重温代码时候非常有用。

使用方法：选中要调整的行，然后按 command+ option + A

**BracketHighlighter**

该插件提供行数列高亮的各种配对的语法符号。（愚人码头注：就是将配对的括号等显示在行数列上）

**Colorpicker**

使用一个取色器改变颜色

使用方法: command + shift + c

注：该插件在Mac上使用时非常漂亮

**Emmet**

Emmet绝对的节省时间。您可以轻松快速地编写HTML。

使用方法: command + option + enter ,并且开始输入Emmet风格的HTML

看看我们的Emmet指南，以了解更多，并自己尝试Emmet。

**DocBlockr**

一个真正简单的方式来轻松地创建许多语言包括JavaScript，PHP和CoffeeScript的文档块。只要在函数的上面输入/**，按Tab就可以了。DocBlockr会观察函数需要的变量名和类型，并创建文档块。

**Git**

Git帮助你与你的Git repo协议进行交互。它支持很多命令像init, push, pull, branch, stash,等的。了解更多关于你在Sublime Text里面究竟能使用哪些Git功能，以提高您的工作流程。https://scotch.io/tutorials/using-git-inside-of-sublime-text-to-improve-workflow

**GitGutter**

这是一个小巧有用的插件，它会告诉你自上次git commit以来已经改变的行。一个指示器显示在行号的旁边。

**Gist**

这个插件可以让你拉你的Gists，并把它们插入到你的文件。当你有一个Gists，以启动一个HTML文件或任何其他可重用的代码时候，这是有用的。

使用方法：打开命令面板，并且键入gist。您也可以使用所显示的快捷方式。

**SidebarEnhancements**

在侧边栏的文件上右击时，这个插件提供了大量更多的选择。打开，查找，复制和粘贴，等等。
这里是老菜单和SidebarEnhanced菜单的比较。

**Themes （主题）**

Sublime Text可以安装主题，有一些主题真的很酷。您可以使用包控制找到这些。

使用包控制安装一个主题，然后更新您的用户设置使用它。

```json
// User/Preferences.sublime-settings
{
	"theme":"Soda Light.sublime-theme"
}
```
注意： 您可能需要重新启动Sublime Text，这些更改才会生效。

**Color Schemes (配色方案)**

除了改变你的主题，你也可以改变你的配色方案。这不同于主题，因为主题是Sublime Text的包。配色方案仅仅是配色方案文件，并更改您的设置。

更改配色方案：菜单，Preferences首选项>Color Scheme配色方案，并选择一个。

个人推荐配色：**[Boxy Theme](https://packagecontrol.io/packages/Boxy%20Theme)** **[Agila Theme](https://packagecontrol.io/packages/Agila%20Theme)** **[Tomorrow Color Schemes](https://packagecontrol.io/packages/Tomorrow%20Color%20Schemes)** **[Theme - Brogrammer](https://packagecontrol.io/packages/Theme%20-%20Brogrammer)** **[Base16 Color Schemes](https://packagecontrol.io/packages/Base16%20Color%20Schemes)**
