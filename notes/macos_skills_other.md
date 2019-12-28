### 小技巧：
1. 浏览器下载的文件名需要Decode的情况：
    ```
        alias urldecode='python -c "import sys, urllib as ul; print ul.unquote_plus(sys.argv[1])"'
        for f in "$@"
        do
          newName=$(urldecode "$f")
          mv "$f" "$newName"
        done
    ```
2. 开启Python SimpleHttpServer
    1. ```sudo apachectl start```
    2. ```python -m SimpleHTTPServer```
    3. [http://localhost:8000](http://localhost:8000)

3.  删除启动台（LaunchPad）中的无效图标
    1. sudo find /private/var/folders/ -name com.apple.dock.launchpad 2>/dev/null
    2. 进入结果文件夹中的db文件夹
    3. 执行`sqlite3 db "delete from apps where title='应用名称';"&&killall Dock`
    
4.  添加路由表
    ```
    sudo route -n add -net 111.199.9.221 -netmask 255.255.255.255 172.20.10.1
    sudo route -n delete -net 111.199.9.221
    ```
5.  MacOS自定义中文文件名映射（类似桌面、文稿）
    1. 打开 Finder，进入 `/System/Library/CoreService/SystemFolderLocalizations/`
    2. 进入 zh_CN.lproj 文件夹，看到下面有一个文件叫 `SystemFolderLocalizations.strings`。字符串就存放在这个文件里。
    3. 把这个文件复制出来
    4. 在10.7之后的系统中是二进制格式的，首先要把它转成XML格式的。`sudo plutil -convert xml1 SystemFolderLocalizations.strings`
    5. 用文本编辑软件打开该文件，添加一行。
    6. 再转换回二进制，`sudo plutil -convert binary1 SystemFolderLocalizations.strings`。
    7. 保存后，重启按住alt，command＋r，后进入终端复制。
    8. 在相应的文件夹中添加文件名是`.localized`的文件。`touch .localized`
    
6. VMware Fusion虚拟机断网解决办法
    1. `sudo /Applications/VMware\ Fusion.app/Contents/Library/vmnet-cli --status`
    2. `sudo /Applications/VMware\ Fusion.app/Contents/Library/vmnet-cli --start`

7. 删除 ABC 输入法
    1. 使用 xCode 编辑`~/Library/Preferences/com.apple.HIToolbox.plist`，删除其中相关 ABC 的所有树形结构
    已知 bug：设置网络手动指定 ip 时，设置页面卡死。