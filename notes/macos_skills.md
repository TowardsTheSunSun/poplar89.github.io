## Mac使用习惯/技巧
###  触摸板
1. 系统偏好设置 —> 触摸板 —> 轻点来点
2. 系统偏好设置 —> 辅助功能 —> 鼠标与触摸板：有鼠标或无线触控板时忽略内建触摸板
    
### 键盘
1. 系统偏好设置 —> 键盘 —> 将F1、F2等键用作标准功能键
2. 系统偏好设置 —> 键盘 —> 快捷键 —> 全键盘控制：选择“所有控制”
3. 系统偏好设置 —> 键盘 —> 快捷键 —> 应用快捷键：去掉“显示帮助菜单”
4. 系统偏好设置 —> 键盘 —> 快捷键 —> 屏幕快照
5. 系统偏好设置 —> 键盘 —> 文本：修改自动纠正
    
### 界面
1. 系统偏好设置 —> 程序坞 —> 将窗口最小化为程序窗口
2. 系统偏好设置 —> 日期与时间：使用24小时格式时钟
3. 系统偏好设置 —> 语言与地区：24小时制
4. 系统偏好设置 -> 键盘 -> 快捷键 -> 新建位于文件夹位置的终端窗口
    
### 聚焦搜索
1. 系统偏好设置 —> 聚焦 —> 去掉不需要的类别
    1. 去掉搜索结果中的代码文件：安装Xcode后，上述设置中去掉"开发者"类别
    2. 上文中对于xcode的安装可以可以使用touch Xcode.app来代替
      
### 启动台 LaunchPad
1. 删除从AppStore安装的引用
    1. 长按图标
    2. ⌥
    
### 安全
1. 系统偏好设置 —> 安全性与隐私 —> 进入睡眠或开始屏幕保护程序“立即”要求输入密码
2. 系统偏好设置 —> 用户与群组 —> 客人用户：不允许客人用户登录到这台电脑
3. 任何来源：```sudo spctl --master-disable```
    
### 网络
1. 系统代理忽略某些主机与域的代理设置：使用英文逗号分隔才生效
        
### [快捷键](../imgs/mac_skills_accelerator_key.png)：
1. 窗口全屏 ⌘ ^ F
2. 全屏窗口之间切换 ^ ←/→
3. Finder中显示隐藏文件：⌘ ⇪ .
4. 锁定屏幕：⌘ ^ Q
5. 同一软件不同窗口之间切换：⌘ \`
6. 输入全角空格 拼音输入法状态下 ⌥ Space
7. Finder中文件剪切
    1. ⌘ C
    2. ⌘ ⌥ V

### 常用软件
1. 隐藏菜单栏不常用图标 Bartender 3
2. 修改快捷键 Karabiner
3. 窗口操作 Window Tidy
4. 快速切换hosts文件 SwitchHosts!
5. 状态栏 iStat Menus
6. 快捷键提示 CheatSheet
7. 隐藏功能工具 TinkerTool
8. 自定义右键菜单 Right Click Booster
9. 屏幕保护时钟 Fliqlo
10. 文件临时存放站 Yoink
11. Youtube 视频下载 iTube、Downie 3
12. 
    
### [小技巧/Scripts](macos_skills_other.md)

### 常见问题
1. 不能完成此操作，因为找不到一个或多个需要的项目。（错误代码 -43）重启Finder
2. [Mac不能按预期睡眠或唤醒](https://support.apple.com/zh-cn/HT204760)
3. Xcode Server Builder无法关闭
    1. Xcode -> Preferences -> Server & Bots -> OFF
    2. Finder进入/Applications/Xcode.app/Contents/Developer/Applications
    3. 将Xcode Server Builder.app 拖入“系统偏好设置 -> 聚焦 -> 隐私”的列表中

备注: 
     ⌘ Command
     ^ Ctrl
     ⇧ Shift
     ⌥ Option
     ⇪ Caps Lock
    
