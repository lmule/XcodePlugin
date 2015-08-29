# XcodePlugin
Xcode作为官方指定的iOS应用开发IDE，功能虽然够用，但用户体验确实一般。

默认的插件安装路径是：`~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins;`，如果不存在，请自动创建。删除插件可以直接从这个目录删除对应的文件夹就可以了。

**ps：安装完插件需要重启Xcode。**

这里主要列举了一些常用的插件。

* [Alcatraz](https://github.com/supermarin/Alcatraz)

    Alcatraz是一个帮你管理Xcode插件、模版以及颜色配置的工具。

    > 安装

    `curl -L http://git.io/lOQWeA | tar xvz -C ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins`

    安装完Alcatraz之后，其他的插件都通过这个安装就可以了。

    **ps：有的插件在最新的Xcode6可能不兼容，需要下载插件工程自助安装。**

* [Auto-Importer](https://github.com/citrusbyte/Auto-Importer-for-Xcode)
    
    可以快速导入头文件。

    > 使用方式
    
    **⌘ + ctrl + H**可以呼出本工程的头文件列表

    ![image](https://github.com/citrusbyte/Auto-Importer-for-Xcode/raw/master/demo.gif)

* [BBUDebuggerTuckAway](https://github.com/neonichu/BBUDebuggerTuckAway)
    
    当你在编辑区域写码的时候，可以自动隐藏Debug Area。

    ![image](https://github.com/neonichu/BBUDebuggerTuckAway/raw/master/plugin.gif)

* [BBUFullIssueNavigator](https://github.com/neonichu/BBUFullIssueNavigator)

    运行工程的时候如果有warning或者error，如果信息很长，最后是省略号，如果你想看完整的信息怎么破？修改如下配置。

    ![image](https://github.com/neonichu/BBUFullIssueNavigator/raw/master/issue-nav-fixed.png)

* [BBUUtilitiesTuckAway](https://github.com/neonichu/BBUUtilitiesTuckAway)

    当你在编辑区域写码的时候，可以自动隐藏Utilities。

    **ps：目前Xcode6.4还不支持，不过作者已经知道这个issue了，近期可能会修复。**

* [Backlight](https://github.com/limejelly/Backlight-for-XCode)

    高亮当前行

    ![image](https://raw.githubusercontent.com/limejelly/Backlight-for-XCode/master/screenshot.png)

    **ps：目前在vim模式下，不高亮**

* [FuzzyAutocomplete](https://github.com/FuzzyAutocomplete/FuzzyAutocompletePlugin)

    根据你的输入能模糊匹配对应的方法、属性

    ![image](https://github.com/FuzzyAutocomplete/FuzzyAutocompletePlugin/raw/master/demo.gif)

* [HTYCopyIssue](https://github.com/hanton/CopyIssue-Xcode-Plugin)

    运行工程的时候如果有warning或者error，如果想直接拷贝issue的信息，而不带文件名和行号，按快捷键**⇧⌘c**，如果想直接搜索，那就直接右键吧。

    **ps：目前只有谷歌和StackOverflow的搜索，但是鉴于谷歌需要自备梯子，所以准备把他的域名换成余老板@leecade 的soulema，此外还会加上百度搜索**
    
    **update：1、更新了谷歌的查询域名；2、因为谷歌的查询结果已经包含了stackoverflow，所以将stackoverflow改成了百度**
    
    `git clone https://github.com/lmule/CopyIssue-Xcode-Plugin.git /tmp/xxxyyy;`
    `cp -r /tmp/xxxyyy/Products/HTYCopyIssue.xcplugin ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins;`

    ![image](https://github.com/hanton/CopyIssue-Xcode-Plugin/raw/master/screenshots/Step1.png?raw=true)

    ![image](https://github.com/hanton/CopyIssue-Xcode-Plugin/raw/master/screenshots/Step2.png?raw=true)

    ![image](https://github.com/hanton/CopyIssue-Xcode-Plugin/raw/master/screenshots/Step2Alternate.png?raw=true)

* [HighlightSelectedString](https://github.com/keepyounger/HighlightSelectedString)

    Xcode高亮显示所有与选中字符串相同的字符串，只是加个虚线，这个插件可以将整个背景高亮

    ![image](https://github.com/keepyounger/HighlightSelectedString/raw/master/demo.png)

* [KSImageNamed](https://github.com/ksuther/KSImageNamed-Xcode)

    当调用[NSImage imageNamed: or [UIImage imageNamed:的时候能自动提示当前Images.xcassests有哪些图片

    ![image](https://camo.githubusercontent.com/c354bf04524df86daeabe7a6d2b9926fac790f85/68747470733a2f2f7261772e6769746875622e636f6d2f6b7375746865722f4b53496d6167654e616d65642d58636f64652f6d61737465722f73637265656e73686f742e676966)

* [SCXcodeTabSwitcher](https://github.com/stefanceriu/SCXcodeTabSwitcher)

    当你受够了每次都要用几个指头前进后退你打开过的文件，或者每次都需要从文件导航窗口去切换文件，那么就需要这个插件了，可以用**⌘cmd + [1..9]**来切换。

    **ps：假如看不到tabbar，可以通过菜单栏View->Show Tab Bar来显示**

    ![image](https://camo.githubusercontent.com/7d875364ccb19ee10b7c1c8d84205c56014936f5/68747470733a2f2f646c2e64726f70626f7875736572636f6e74656e742e636f6d2f752f31323734383230312f5265636f7264696e67732f534358636f646554616253776974636865722f534358636f646554616253776974636865722e676966)

* [VVDocumenter-Xcode](https://github.com/onevcat/VVDocumenter-Xcode)

    自动生成注释神器，在方法上面直接输入**///**就可以生成注释了。

    ![image](https://camo.githubusercontent.com/ca5518c9872e15b8a95b9d8c5f44bc331977d710/68747470733a2f2f7261772e6769746875622e636f6d2f6f6e65766361742f5656446f63756d656e7465722d58636f64652f6d61737465722f53637265656e53686f742e676966)

* [XLCXcodeAssist](https://github.com/xlc/XLCXcodeAssist)

    在继承protocol的时候，如果你没有一辉的手速，那么就可以使用这个插件来自动实现protocol必须要实现的方法。但现在只支持objective-c自带的protocol，比如UITableViewDataSource、UITableViewDelegate

    ![image](https://raw.githubusercontent.com/xlc/XLCXcodeAssist/master/images/method.png)

    还可以自动补全switch、if这种代码片段

    ![image](https://raw.githubusercontent.com/xlc/XLCXcodeAssist/master/images/switch.png)

* [XVim](https://github.com/XVimProject/XVim)

    Xcode的vim模式
