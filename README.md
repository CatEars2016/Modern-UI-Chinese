# Modern UI for WPF (MUI) Chinese Support
源项目：[https://github.com/firstfloorsoftware/mui](https://github.com/firstfloorsoftware/mui)

使用Modern UI for WPF时发现中文字体显示效果较差且不可修改，于是下载它的源码进行修改。

【2019-02-16】修改内容：
* 将logo的显示位置移动到窗口左上角。
* 如果设置了Icon属性但未设置LogoData属性，将会在logo的位置上显示Icon
* 增加资源MenuFontSize和SubMenuFontSize用于调整菜单字体大小(因为子菜单字体太小了)
* 去掉SubMenu选中时字体加粗。(因为用在中文上效果不好)
* 去掉ToUpperConverter和ToLowerConverter等2个转换器。(因为中文中含有英文时，多数情况不希望变大写或者变小写)

【2019-02-10】修改内容：
* 【解决Segoe UI显示中文字体效果较差的问题】
  * 所有"Segoe UI"字体换成"{DynamicResource DefaultFontFamily}"。
  * 增加字体资源LightFontFamily，所有"Segoe UI Light"字体换成"{DynamicResource LightFontFamily}"。
* 增加中文语言支持（Resources.zh.resx），取消其它外语语言。
* ModernWindow增加IsBackButtonVisible属性，默认值True。


# Modern UI for WPF (MUI)
A set of controls and styles converting your WPF application into a great looking Modern UI app. This open source project is a spin-off of [XAML Spy](http://xamlspy.com), the visual runtime inspector for Silverlight, Windows Phone, Windows Store and WPF. Read the [official announcement](http://xamlspy.com/news/open-sourcing-the-xaml-spy-ui)

[![Build status](https://img.shields.io/appveyor/ci/kozw/mui.svg)](https://ci.appveyor.com/project/kozw/mui)
[![Release](https://img.shields.io/github/release/firstfloorsoftware/mui.svg)](https://github.com/firstfloorsoftware/mui/releases/latest)
[![NuGet](https://img.shields.io/nuget/dt/ModernUI.WPF.svg)](http://nuget.org/packages/ModernUI.WPF)
[![Stars](https://img.shields.io/github/stars/firstfloorsoftware/mui.svg)](https://github.com/firstfloorsoftware/mui/stargazers)

## Demo
Check out the **MUI demo app** included in the [MUI release](https://github.com/firstfloorsoftware/mui/releases). The app demonstrates most features of the MUI framework. The [full source](https://github.com/firstfloorsoftware/mui/tree/master/1.0/FirstFloor.ModernUI/FirstFloor.ModernUI.App) of the demo app is included in the source code of this project.

## Documentation
See some [screenshots](https://github.com/firstfloorsoftware/mui/wiki/Screenshots) to get an idea of what Modern UI for WPF is all about. And visit the [wiki](https://github.com/firstfloorsoftware/mui/wiki) to learn how to incorporate Modern UI for WPF into your application.

![](http://firstfloorsoftware.com/media/github/mui/mui.intro.png)

## Features
* Appearance, configurable at runtime
  * Dark, light and custom themes
  * Accent color
  * Large and small fonts
* New modern controls
  * BBCodeBlock
  * ModernButton
  * ModernDialog
  * ModernFrame
  * ModernMenu
  * ModernProgressRing (with 8 built-in styles)
  * ModernTab
  * ModernToggleButton
  * ModernWindow
  * RelativeAnimatingContentControl
  * TransitioningContentControl
* Layout
  * A set of predefined page layouts for a consistent look & feel
* Control styles
  * Styles for common WPF controls, such as Button, TextBlock, etc.
  * All styles automatically adapt the dark and light theme and use accent colors where appropiate
* Customizable navigation framework
  * ILinkNavigator and IContentLoader interfaces for maximum flexibility
  * Content loader exception templates in ModernFrame
* Project and item templates
  * Visual Studio 2012, 2013 and 2015 project and item templates for creating ModernUI apps as fast and smooth as possible
  * Read more and download the extension containing the templates from the [Visual Studio Gallery](http://visualstudiogallery.msdn.microsoft.com/7a4362a7-fe5d-4f9d-bc7b-0c0dc272fe31)

## Acknowledgements
* [WPF Shell Integration Library](http://archive.msdn.microsoft.com/WPFShell)
* Adapted the TransitioningContentControl from [WPF Toolkit](http://wpf.codeplex.com/)
* Adapted the Windows Phone [RelativeAnimatingContentControl](http://msdn.microsoft.com/en-us/library/gg442303(v=vs.92).aspx) for custom indeterminate ProgressBar styling
* ModernProgressRing styles taken from https://github.com/nigel-sampson/spinkit-xaml
* Modern button icons in sample app taken from http://modernuiicons.com/

