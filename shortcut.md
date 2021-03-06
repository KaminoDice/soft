# 快捷键方案

在我看来, 快捷键的目的是尽量减少手的移动, 从而提升效率.
- 总在鼠标/键盘切换感觉好累, 而且一直用 鼠标/小红点/触摸板 感觉对 手指/手腕 很不友好
- 不可否认, 某些情况下鼠标操作更加方便, 所以不要盲目迷信快捷键

## 一般准则
规范准则
1. Keep simply. 为保证此准则, 尽量参照如下原则:
    - 保证操作的粒度足够小
    - 使用lazy模式, 不做目前不需要的可有可无的添加
2. 当自己没有一套成熟的快捷键方案时, 可以参考 vim 的快捷键方案
本文主要是介绍基于 vim 的快捷键方案

学习建议
1. 保持兴趣最重要, 如果你觉得vim很难, 没关系, 先在你所使用的ide下装个vim插件使用, 慢慢来. 谨记保持热情才能走的更远.

一些可以自定义快捷键的软硬件
1. ArchLinux + i3wm: 不可否认的是, 除了纯终端大佬, 其他无论是 win/os, 还是各linux发行版, 都不可能只使用键盘. 但是, 我还是比较推荐 arch+i3wm 的组合, 原因如下:
    - arch 本身不带任何可有可无的软件, 也就是说不带界面, 如此从一开始我们得到的就是一个纯净的系统, 在此之上我们可以自定义快捷键等各方面设置.
    - i3wm 桌面可以通过设置任意快捷键实现 跳转/切换 至任意桌面. 详细参考 [i3_arch文档](https://wiki.archlinux.org/index.php/i3_(简体中文)).
2. chrome + vimium: chrome 应该是大多数开发者的标配浏览器了吧, vimium 插件可以让你在一定程度上按照 vim 的快捷键方案使用chrome.
3. vscode + vim: 同上
4. ikbc poker: ikbc 的一款67键键盘, 支持可编程, 之所以不推荐 hhkb, 是因为个人还是很不适应hhkb类似薄膜键盘的手感. 而且, poker以及类似的键盘至少可以通过改键值实现相应的功能, 所以 hhkb 对我的诱惑不大.

## 快捷键方案
一般规律
1. 方向键方案
    - wasd => 方向键
    - hjkl => 方向键
2. 不同软件/模式使用不同的关键字层, 如 i3 使用 $mod 键作为层按键, vimium没有必要
3. 不同层下, 方便快捷的按键时不同的, 所以不是所有层标准一定要一致, 而是尽量保持一致
4. 大写模式一般用于小写模式的扩展, 加shift是原模式的扩展
5. 指令单元最小化, 组合指令使用

### vim快捷键
[vim常用快捷键列表](/develop/vim/shortcuts.md)

### i3快捷键
i3wm 快捷键方案: 编程层: $mod
1. 具体配置请参照i3wm配置文件. [配置文件](/os/arch/config/i3/config)
2. `$mod+tab` 作为 termite window 的切换快捷键
2. `$mod+e` 作为 quikefix(即scrapad) 的快捷键
3. `$mod+q` 作为 rofi 窗口查询的快捷键

### vimium
vim 基于 chrome 的vim插件.

参考 https://sspai.com/post/27723

常用指令: 支持 hjklgG 等vim命令

| 作用              | 指令  | 详解                |
|-----------------|-----|-------------------|
| 左右切换tab         | J/K | 大写的jk             |
| 打开页面链接          | f/F | f: 当页打开,F: 新标签页打开 |
| 新页打开url/书签/历史记录 | t   | tabNew(使用tab切换选项) |
| 当页打开url/书签/历史记录 | o   | open(使用tab切换选项)   |
| 复制当前url         | yy  | 与vim同             |
| 打开复制的页面         | p/P | 当页/新标签            |
| 翻滚半屏            | d/u |                   |

组合使用

| 作用      | 指令  | 详解  |
|---------|-----|-----|
| 复制链接url | yf  | y+f |

chrome 快捷键

| 作用     | 指令            | 详解            |
|--------|---------------|---------------|
| 切换焦点   | f6            | 输入栏/书签/正文焦点切换 |
| 前进/后退  | alt+方向键       |               |
| 移动标签位置 | alt+shift+方向键 |               |

### poker键盘
poker键盘快捷键方案: 编程层: Fn
1. CapsLock 映射为 Fn
