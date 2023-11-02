<!--suppress HtmlDeprecatedAttribute, HttpUrlsUsage -->

<div align="center">
  <p>
    <img src="https://s1.imagehub.cc/images/2023/03/07/af8ed087c9d354b9ab6142aae7bbafb6.png" alt="autojs6-banner_800×224" border="0" width="704" />
  </p>

  <p>Android 平台支持无障碍服务的 JavaScript 自动化工具</p>

  <p>
    <a href="http://download.autojs6.com"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/SuperMonster003/AutoJs6"/></a>
    <a href="http://issues.autojs6.com"><img alt="GitHub closed issues" src="https://img.shields.io/github/issues/SuperMonster003/AutoJs6?color=009688"/></a>
    <a href="http://commit.autojs6.com/99a1d8490fac5b6d55f6f183db59ad833a2064ed"><img alt="Created" src="https://img.shields.io/date/1636632233?color=2e7d32&label=created"/></a>
    <br>
    <a href="https://github.com/mozilla/rhino"><img alt="Rhino" src="https://img.shields.io/badge/rhino-1.7.15--snapshot-F06292"/></a>
    <a href="https://developer.android.com/studio/archive"><img alt="Android Studio" src="https://img.shields.io/badge/android%20studio-2022.1+-B64FC8"/></a>
    <br>
    <a href="https://www.codefactor.io/repository/github/SuperMonster003/AutoJs6"><img alt="CodeFactor Grade" src="https://www.codefactor.io/repository/github/SuperMonster003/AutoJs6/badge"/></a>
    <a href="http://project.autojs6.com/find/master"><img alt="GitHub Code Size" src="https://img.shields.io/github/languages/code-size/SuperMonster003/AutoJs6?color=795548"/></a>
    <a href="http://project.autojs6.com/blob/master/LICENSE"><img alt="GitHub License" src="https://img.shields.io/github/license/SuperMonster003/AutoJs6?color=534BAE"/></a>
  </p>
</div>

******

### 简介

******

[Auto.js](https://github.com/hyb1996/Auto.js) 是一款 Android 平台支持 [无障碍服务](https://developer.android.com/guide/topics/ui/accessibility/service?hl=zh-cn) 的 JavaScript 自动化工具软件.

Auto.js 由 [hyb1996](https://github.com/hyb1996) 于 `2017/01/27` 初次发布, 于 `2020/03/13` 停止维护, 最终版本名称为 `4.1.1 alpha2`.

AutoJs6 在 Auto.js 最终项目的基础上, 于 `2021/12/01` 进行二次开发, 继续保持开源免费.

基于 Auto.js 二次开发的开源项目 (以开发时间排序, 仅部分列举):

|                         项目名称                          |          应用名称          |                          开发者                          |     开发时间     |
|:-----------------------------------------------------:|:----------------------:|:-----------------------------------------------------:|:------------:|
|   [Auto.js](https://github.com/TonyJiangWJ/Auto.js)   |       Auto.js M        |     [TonyJiangWJ](https://github.com/TonyJiangWJ)     | `2019/11/21` |
|      [AutoX](https://github.com/kkevsekk1/AutoX)      | Autox.js / Autox.js v6 |       [kkevsekk1](https://github.com/kkevsekk1)       | `2020/07/24` |
| [AutoJs6](https://github.com/SuperMonster003/AutoJs6) |        AutoJs6         | [SuperMonster003](https://github.com/SuperMonster003) | `2021/12/01` |

******

### 功能

******

* 可用作 JavaScript IDE (代码补全/变量重命名/代码格式化)
* 支持基于 [无障碍服务](https://developer.android.com/reference/android/accessibilityservice/AccessibilityService) 的自动化操作
* 支持浮动按钮快捷操作 (脚本录制及运行/查看包名及活动/布局分析)
* 支持选择器 API 并提供控件遍历/获取信息/控件操作 (类似 [UiAutomator](https://developer.android.com/training/testing/ui-automator))
* 支持布局界面分析 (类似 Android Studio 的 LayoutInspector)
* 支持录制功能及录制回放
* 支持屏幕截图/保存截图/图片找色/图片匹配
* 支持 [E4X](https://zh.wikipedia.org/wiki/E4X) (ECMAScript for XML) 编写界面
* 支持将脚本文件或项目打包为 APK 文件
* 支持利用 Root 权限扩展功能 (屏幕点击/滑动/录制/Shell)
* 支持作为 Tasker 插件使用
* 支持与 VSCode 连接并进行桌面开发 (需要 [AutoJs6-VSCode-Extension](http://vscext-project.autojs6.com) 插件)

******

### 环境

******

- Android 操作系统
- [API](https://developer.android.com/guide/topics/manifest/uses-sdk-element#ApiLevels) [24](https://developer.android.com/reference/android/os/Build.VERSION_CODES#N) ([7.0](https://zh.wikipedia.org/wiki/Android_Nougat)) [[N](https://developer.android.com/reference/android/os/Build.VERSION_CODES#N)] 及以上

******

### 指南

******

* [应用文档](https://docs.autojs6.com)
* [使用手册 (待编写)](https://docs.autojs6.com/#/manual)
* [疑难解答](https://docs.autojs6.com/#/qa)
* [项目编译构建](#项目编译构建)
* [脚本开发辅助](#脚本开发辅助)

******

### 主要变更

******

* VSCode 插件支持客户端 (LAN) 及服务端 (LAN/ADB) 连接方式

* 多语言适配 (西/法/俄/阿/日/韩/英/简中/繁中等)

* 夜间模式适配 (设置页面/文档页面/布局分析页面/浮动窗口等)

* [Rhino](https://github.com/mozilla/rhino/) 引擎由 [v1.7.7.2](https://github.com/mozilla/rhino/releases/tag/Rhino1_7_7_2_Release) 升级至 [v1.7.15-SNAPSHOT](http://rhino.autojs6.com/blob/dbe3f43ba5eb01e7f76139208f36c383dcd1c488/gradle.properties#L3)

    * 支持 [Object.values()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/values)

       ```javascript
       Object.values({name: 'Max', age: 4}); // ['max', 4]
       ```

    * 支持 [Array.prototype.includes()](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Array/includes)

       ```javascript
       [10, 20, NaN].includes(20); // true
       ```

    * 支持 [BigInt](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/BigInt)

       ```javascript
       typeof 567n === 'bigint'; // true
       ```

    * 支持 [模板字符串](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Template_literals)

       ```javascript
       `Lucky number: ${(Math.random() * 100).toFixed(0)}`
       ```

    * 查看 Rhino 引擎 [更多新特性](http://project.autojs6.com/blob/master/app/src/main/assets/doc/RHINO.md)

    * 查看 Rhino 引擎 [兼容性列表](https://mozilla.github.io/rhino/compat/engines.html)

******

### 版本历史

******

[comment]: <> "Version history only shows last 3 versions"

# v6.4.1

###### 2023/11/02

* `修复` 构建工具无法自适应未知平台的问题 (by [TonyJiangWJ](https://github.com/TonyJiangWJ)) _[`pr #158`](http://pr.autojs6.com/158)_
* `修复` 脚本退出时可能导致应用崩溃的问题 _[`issue #159`](http://issues.autojs6.com/159)_
* `修复` http 模块获取响应对象的 body.contentType 返回值类型错误 _[`issue #142`](http://issues.autojs6.com/142)_
* `修复` device.width 及 device.height 返回数据不正确的问题 _[`issue #160`](http://issues.autojs6.com/160)_
* `修复` 代码编辑器长按删除时可能导致应用崩溃的问题 (试修) _[`issue #156`](http://issues.autojs6.com/156)_
* `修复` 代码编辑器反向选择文本后进行常规操作可能导致应用崩溃的问题
* `修复` 部分设备长按 AutoJs6 应用图标无法显示快捷方式菜单的问题
* `修复` 部分设备打包项目时点击确认按钮无响应的问题
* `修复` app.sendBroadcast 及 app.startActivity 无法使用简称参数的问题
* `修复` floaty 模块 JsWindow#setPosition 等方法首次调用时的功能异常
* `优化` 增加 Termux 相关权限以支持 Intent 调用 Termux 执行 ADB 命令 _[`issue #136`](http://issues.autojs6.com/136)_
* `优化` http 模块获取的响应对象可重复使用 body.string() 及 body.bytes() 方法
* `优化` 增加 GitHub Actions 自动打包支持 (by [TonyJiangWJ](https://github.com/TonyJiangWJ)) _[`pr #158`](http://pr.autojs6.com/158)_
* `优化` 构建工具自适应 Temurin 平台
* `优化` 部分依赖或本地库版本调整 _[`CHANGELOG.md`](http://project.autojs6.com/blob/master/app/src/main/assets/doc/CHANGELOG.md#v641)_

# v6.4.0

###### 2023/10/30

* `新增` ocr 模块支持 Paddle Lite 引擎 (by [TonyJiangWJ](https://github.com/TonyJiangWJ)) _[`pr #120`](http://pr.autojs6.com/120)_
* `新增` 打包功能支持内置插件与外部插件两种打包方式 (by [LZX284](https://github.com/LZX284)) _[`pr #151`](http://pr.autojs6.com/151)_
* `新增` WebSocket 模块 (参阅 项目文档 > [WebSocket](https://docs.autojs6.com/#/webSocketType))
* `新增` barcode / qrcode 模块 (参阅 项目文档 > [条码](https://docs.autojs6.com/#/barcode) / [二维码](https://docs.autojs6.com/#/qrcode))
* `新增` shizuku 模块 (参阅 项目文档 > [Shizuku](https://docs.autojs6.com/#/shizuku)) 及主页抽屉权限开关
* `新增` device.rotation / device.orientation 等方法
* `新增` 内部 Java 类支持 class 静态属性访问
* `新增` 支持在安卓系统设置页面选择并切换应用语言 (安卓 13 及以上)
* `新增` 支持设置页面添加或长按应用图标激活 [应用快捷方式](https://developer.android.com/guide/topics/ui/shortcuts?hl=zh-cn) , 可启动文档和设置等页面
* `修复` 重新合并部分 PR (by [aiselp](https://github.com/aiselp)) 以解决部分脚本无法正常结束运行的问题 _[`pr #75`](http://pr.autojs6.com/75)_ _[`pr #78`](http://pr.autojs6.com/78)_
* `修复` 打包应用无法使用 AutoJs6 新增 API 的问题 (by [LZX284](https://github.com/LZX284)) _[`pr #151`](http://pr.autojs6.com/151)_
* `修复` 打包应用在系统夜间模式下的样式异常
* `修复` VSCode 插件保存文件到本地时文件扩展名信息丢失的问题
* `修复` 使用协程特性运行项目产生未捕获异常致使应用崩溃的问题
* `修复` 重启或退出应用时浮动按钮无法记录其位置状态信息的问题
* `修复` 设备屏幕方向改变时无法获取更新后的设备配置信息的问题 _[`issue #153`](http://issues.autojs6.com/153)_
* `修复` 屏幕旋转至横向时 Toolbar 标题字体过小的问题
* `修复` 屏幕旋转至横向时应用主页的页签排版过于拥挤的问题
* `修复` 屏幕旋转至横向时浮动按钮可能溢出屏幕的问题 _[`issue #90`](http://issues.autojs6.com/90)_
* `修复` 屏幕多次旋转时无法恢复浮动按钮的坐标及屏幕侧边方向的问题
* `修复` 部分设备消息浮动框可能出现遗漏显示或重复显示的问题
* `修复` 消息浮动框在多个脚本同时运行时可能存在被遮蔽的问题 _[`issue #67`](http://issues.autojs6.com/67)_
* `修复` 使用广播分析布局时点击布局无法弹出菜单且导致应用崩溃的问题
* `修复` 第二次及以后创建的 WebSocket 实例均无法正常触发监听器的问题
* `修复` 撤销 importPackage 的全局重定向方法以避免某些作用域下的包导入异常 _[`issue #88`](http://issues.autojs6.com/88)_
* `修复` 日志活动页面使用复制或导出功能时可能导致应用崩溃的问题
* `优化` 日志活动页面导出功能重命名为发送功能并重新实现符合实际意义的导出功能
* `优化` 日志活动页面发送功能支持条目数量过大时自动截取并作出提示
* `优化` ocr 模块同时兼容 Google MLKit 及 Paddle Lite 引擎 (参阅 项目文档 > [光学字符识别](https://docs.autojs6.com/#/ocr?id=p-mode))
* `优化` 提升无障碍服务自动启动的成功概率
* `优化` Kotlin 注解处理由 kapt 迁移至 KSP
* `优化` 构建工具支持 IntelliJ Idea EAP 版本
* `优化` 构建工具自适应 Java 发行版本以尽量避免 "无效的发行版本" 问题
* `优化` 构建工具优化 IDE 及相关插件的版本退级逻辑并增加版本预测能力
* `优化` 适配 VSCode 插件 1.0.7
* `优化` 部分依赖或本地库版本调整 _[`CHANGELOG.md`](http://project.autojs6.com/blob/master/app/src/main/assets/doc/CHANGELOG.md#v640)_

# v6.3.3

###### 2023/07/21

* `新增` 代码编辑器的代码注释功能 (by [抠脚本人](https://github.com/little-alei)) _[`pr #98`](http://pr.autojs6.com/98)_
* `新增` auto.stateListener 用于无障碍服务连接状态监听 (by [抠脚本人](https://github.com/little-alei)) _[`pr #98`](http://pr.autojs6.com/98)_
* `新增` UiObject 类型添加 nextSibling / lastChild / offset 等方法 (参阅 项目文档 > [控件节点](https://docs.autojs6.com/#/uiObjectType))
* `修复` VSCode 插件在脚本字符总长度超过四位十进制数时无法解析数据的问题 _[`issue #91`](http://issues.autojs6.com/91)_ _[`issue #93`](http://issues.autojs6.com/93)_ _[`issue #100`](http://issues.autojs6.com/100)_ _[`issue #109`](http://issues.autojs6.com/109)_
* `修复` VSCode 插件无法正常保存文件的问题 _[`issue #92`](http://issues.autojs6.com/91)_ _[`issue #94`](http://issues.autojs6.com/93)_
* `修复` 浮动按钮菜单项 "管理无障碍服务" 点击后可能未发生页面跳转的问题
* `修复` runtime.requestPermissions 方法丢失的问题 _[`issue #104`](http://issues.autojs6.com/104)_
* `修复` events.emitter 不支持 MainThreadProxy 参数的问题 _[`issue #103`](http://issues.autojs6.com/103)_
* `修复` 在 _[`pr #78`](http://pr.autojs6.com/78)_ 中存在的代码编辑器无法格式化代码的问题
* `修复` 使用 JavaAdapter 时导致 ClassLoader 调用栈溢出的问题 _[`issue #99`](http://issues.autojs6.com/99)_ _[`issue #110`](http://issues.autojs6.com/110)_
* `优化` 调整模块作用域 (by [aiselp](https://github.com/aiselp)) _[`pr #75`](http://pr.autojs6.com/75)_ _[`pr #78`](http://pr.autojs6.com/78)_
* `优化` 移除发行版本应用启动时的签名校验 (by [LZX284](https://github.com/LZX284)) _[`pr #81`](http://pr.autojs6.com/81)_
* `优化` 在 _[`pr #98`](http://pr.autojs6.com/98)_ 基础上的编辑器代码注释功能的行为, 样式及光标位置处理
* `优化` 在 _[`pr #98`](http://pr.autojs6.com/98)_ 基础上添加代码注释菜单项
* `优化` 适配 VSCode 插件 1.0.6
* `优化` UiObject#parent 方法增加级数参数支持 (参阅 项目文档 > [控件节点](https://docs.autojs6.com/#/uiObjectType))

##### 更多版本历史可参阅

* [CHANGELOG.md](http://changelog.autojs6.com)

******

### 项目编译构建

******

如需对 AutoJs6 开源项目进行调试或开发, 可使用 Android Studio 或 [IntelliJ IDEA](https://www.jetbrains.com/idea/) ([Jetbrains](https://www.jetbrains.com/) 公司产品).

本小节以 Android Studio 为例介绍 AutoJs6 开源项目的编译构建方法, IntelliJ IDEA 与之类似.

#### Android Studio 准备

下载 `Android Studio Hedgehog | 2023.1.1 RC 2` 版本 (按需选择其一):

- [android-studio-2023.1.1.24-windows.exe](https://redirector.gvt1.com/edgedl/android/studio/install/2023.1.1.24/android-studio-2023.1.1.24-windows.exe) (1.1 GB)
- [android-studio-2023.1.1.24-windows.zip](https://redirector.gvt1.com/edgedl/android/studio/ide-zips/2023.1.1.24/android-studio-2023.1.1.24-windows.zip) (1.1 GB)

> 注: 上述版本发布时间为 2023 年 10 月 30 日. 如需下载其他版本, 或上述链接已失效, 可访问 [Android Studio 发行版本归档](https://developer.android.com/studio/archive?hl=en) 页面.

安装或解压上述文件, 运行 Android Studio 软件 (如 `"D:\android-studio\bin\studio64.exe"`).

#### Android SDK 准备

> 注: 如果计算机系统已安装 Android SDK (安卓软件开发工具包), 则可跳过此小节内容.

在 Android Studio 软件中使用快捷键 `CTRL + ALT + S` 打开设置页面:

```text
Appearance & Behavior (外观与表现) -> 
System Settings (系统设置) -> 
Android SDK (安卓软件开发工具包)
```

`Android SDK Location (安卓软件开发工具包位置)` 处如果是空白内容, 可点击右侧 `Edit (编辑)` 按钮, 在弹出的窗口中多次点击 `Next (下一步)`.

> 注: 过程中可能需要同意一个或多个相关协议才能继续.

待相关资源下载并安装完毕, 点击 `Finish (完成)` 按钮.  
上述 `Android SDK Location (安卓软件开发工具包位置)` 处将自动完成路径填写, SDK 准备工作随即完成.

#### Android SDK Tools 准备

AutoJs6 需要使用部分 SDK 工具 (如 NDK 及 CMake).

> 注: 如果计算机系统已安装 AutoJs6 全部所需的 Android SDK Tools, 则可跳过此小节内容.

在 Android Studio 软件中使用快捷键 `CTRL + ALT + S` 打开设置页面:

```text
Appearance & Behavior (外观与表现) -> 
System Settings (系统设置) -> 
Android SDK (安卓软件开发工具包) -> 
SDK Tools (SDK 工具) (位于右侧窗口)
```

勾选 `Show Package Details (显示包详情)`, 依次点击 NDK 及 CMake, 确保相应版本的工具已勾选 (截至 2023 年 10 月 30 日, NDK 所需版本为 `21.1.6352462`, CMake 所需版本为 `3.10.2`).

SDK 工具的版本信息位于 AutoJs6 项目根目录的 `version.properties` 文件中.

#### JDK 准备

AutoJs6 项目依赖的 `JDK (Java 开发工具包)` 发行版本不低于 `17`, 但建议不低于 `19`.

需额外留意, 截至 2023 年 10 月 30 日, AutoJs6 暂不支持 JDK 最新版本 `21`.

> 注: 如果计算机系统已安装 JDK 且版本满足上述要求, 则可跳过此小节内容.

JDK 可使用 IDE 直接下载, 或访问 [Oracle 网站](https://www.oracle.com/java/technologies/downloads/) 下载.

在 Android Studio 软件中使用快捷键 `CTRL + ALT + S` 打开设置页面:

```text
Build, Execution, Deployment (构建, 执行, 开发) ->
Build Tools (构建工具) -> 
Gradle
```

`Gradle JDK` 处可选择或添加不同版本的 JDK.

如果列表中已存在合适版本的 JDK (>= `17`), 则直接选择即可.  
否则可以选择 `Download JDK (下载 JDK)` 下载合适的 JDK, 点击 `Download (下载)` 按钮并等待下载完成.  
也可以选择 `Add JDK (添加 JDK)` 添加已存在的本地 JDK, 定位其目录并完成 JDK 添加.

#### AutoJs6 资源克隆

在 Android Studio 主页面点击 `Get from VCS (从版本控制系统获取)` 按钮.  
`URL (统一资源定位地址)` 处填入 `https://github.com/SuperMonster003/AutoJs6.git`,  
`Directory (目录)` 处可根据需要修改为特定路径.  
点击 `Clone (克隆)` 按钮, 等待 AutoJs6 项目资源在设备本地完成克隆.

> 注: 上述过程可能需要安装 [Git (分布式版本控制系统)](https://git-scm.com/download).

#### AutoJs6 项目构建

克隆完成后, Android Studio 将打开 AutoJs6 的项目窗口, 并自动完成初步的 `Dependencies (依赖)` 下载及 Gradle 构建工作.

> 注: 上述过程可能非常耗时. 若网络条件欠佳, 可能需要重试多次 (点击 Retry 按钮).

构建完成后, Android Studio 的 `Build` 标签页将出现类似 `BUILD SUCCESSFUL in 1h 17m 34s` 的消息.

打包项目并生成可安装到安卓设备的 APK 文件:

- 调试版 (Debug Version)
    - `Build (构建)` -> `Build Bundle(s) / APK(s)` -> `Build APK(s)`
    - 生成带默认签名的调试版安装包
    - 路径示例: `"D:\AutoJs6\app\build\outputs\apk\debug\"`
- 发布版 (Release Version)
    - `Build (构建)` -> `Generate Signed Bundle / APK`
    - 选择 `APK` 选项
    - 准备好签名文件 (新建或选取), 生成已签名的发布版安装包
    - 路径示例: `"D:\AutoJs6\app\release\"`

> 参阅: [Android Docs](https://developer.android.com/studio/run?hl=zh-cn)

******

### 脚本开发辅助

******

开发 AutoJs6 可运行的脚本, 需使用合适的开发工具:

- [VSCode](https://code.visualstudio.com/download) / [WebStorm](https://www.jetbrains.com/webstorm/download/) / [HBuilderX](https://www.dcloud.io/hbuilderx.html) ...

如需在 PC 上进行脚本编写与调试, VSCode 插件可以实现 PC 与手机的互联:

- [AutoJs6-VSCode-Extension](http://vscext-project.autojs6.com) - AutoJs6 调试器 (VSCode 平台插件)

使用开发工具编写代码时, 代码智能补全功能可以更好地辅助开发者完成代码编写:

- [AutoJs6-TypeScript-Declarations](http://dts-project.autojs6.com) - AutoJs6 声明文件 (代码智能补全)

编写代码时, AutoJs6 相关 API 及使用方式, 可随时查阅应用文档:

- [AutoJs6-Documentation](http://docs-project.autojs6.com) - AutoJs6 应用文档

现有的脚本开发项目可作为参考, 激发个人脚本项目的创作灵感:

- [Ant-Forest](https://github.com/TonyJiangWJ/Ant-Forest) - 蚂蚁森林能量自动收取脚本 by [TonyJiangWJ](https://github.com/TonyJiangWJ)
- [Ant-Forest](https://github.com/SuperMonster003/Ant-Forest) - 蚂蚁森林能量自动收取脚本 by [SuperMonster003](https://github.com/SuperMonster003)
- [autojs](https://github.com/e1399579/autojs) - Auto.js 实用脚本 by  [e1399579](https://github.com/e1399579)
- [autojsDemo](https://github.com/snailuncle/autojsDemo) - Auto.js 演示示例 by  [snailuncle](https://github.com/snailuncle)
- [autojs 相关仓库](https://github.com/topics/autojs) - GitHub 与 autojs 话题相关的全部仓库

******

### 贡献参与

******

感谢每一位参与 AutoJs6 项目开发的贡献人员.

|                         贡献人员                          |                                       提交数                                       |     最近提交     |
|:-----------------------------------------------------:|:-------------------------------------------------------------------------------:|:------------:|
|     [TonyJiangWJ](https://github.com/TonyJiangWJ)     |   [4](https://github.com/SuperMonster003/AutoJs6/commits?author=TonyJiangWJ)    | `2023/10/31` |
|       [LZX284](https://github.com/LZX284) (Ai)        |     [13](https://github.com/SuperMonster003/AutoJs6/commits?author=LZX284)      | `2023/10/09` |
| [little-alei](https://github.com/little-alei) (抠脚本人)  |   [12](https://github.com/SuperMonster003/AutoJs6/commits?author=little-alei)   | `2023/07/12` |
|          [aiselp](https://github.com/aiselp)          | [6](https://github.com/SuperMonster003/AutoJs6/pulls?q=is%3Apr+author%3Aaiselp) | `2023/06/14` |
|        [LYS86](https://github.com/LYS86) (LYS)        |      [2](https://github.com/SuperMonster003/AutoJs6/commits?author=LYS86)       | `2023/06/03` |

数据更新于 `2023/10/31`.

数据条目按 `最近提交` 降序排序.

新发起的暂未处理的 Pull Request, 将在合并处理后加入数据统计.

部分贡献人员在 [GitHub Contributors](https://github.com/SuperMonster003/AutoJs6/graphs/contributors) 未能正常出现, 其提交记录为空, 仍可通过 [Pull Request](https://github.com/SuperMonster003/AutoJs6/pulls) 查看贡献记录.

[//]: # (
    # --------------------------------------------------------------#
    # Before committing and pushing to the remote GitHub repository #
    # --------------------------------------------------------------#
    - CHANGELOG.md
        - Update entries for AutoJs6 by checking all changed files
        - Update entries for Gradle plugins [ implementation ]
        - Update version name and released date
        - Append related GitHub issues to changelog entries
    - README.md
        - Latest changelog was synchronized by which in CHANGELOG.md
        - Changelog entries are not more than three
        - The summary of the latest changelog for committing to Git [ DO NOT commit or push ]
        - Update badges like [ android studio / rhino / ... ]
        - Update android studio download links and version names
    - Remove the part like [ alpha / beta / ... ] of VERSION_NAME in version.properties
    - Update dependencies information for Android Gradle Plugin in the top-level build.gradle.kts
    - Update dependencies TypeScript declarations.
    - Re-generate documentation by running the python script
    - Check the two-way versions for AutoJs6 and VSCode ext, then publish the ext to Microsoft
    - Run Gradle task "app:assembleInrtRelease"
    - Build APK to determine the final VERSION_BUILD field
    - Commit and push to GitHub
)
