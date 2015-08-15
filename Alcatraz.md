# Alcatraz
Alcatraz是一个帮你管理Xcode插件、模版以及颜色配置的工具。它可以直接集成到Xcode的图形界面中，让你感觉就像在使用Xcode自带的功能一样。

> 安装

`mkdir -p ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins;`

`curl -L http://git.io/lOQWeA | tar xvz -C ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins`

> 删除

`rm -rf ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins/Alcatraz.xcplugin`

`rm -rf ~/Library/Application\ Support/Alcatraz`

> 使用

安装成功后重启Xcode，就可以在Xcode的顶部菜单中找到Alcatraz，如下所示：
![image](https://cloud.githubusercontent.com/assets/10286518/9289836/e11db7ac-43ae-11e5-9120-02c9054bc3ff.png)

点击“Package Manager”，即可启动插件列表页面，如下所示：
![image](https://cloud.githubusercontent.com/assets/10286518/9289851/6bdcab8c-43af-11e5-8696-fee891b0fcc5.png)

Xcode所有的插件都安装在目录`~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins/`下，你也可以手工切换到这个目录来删除插件。


