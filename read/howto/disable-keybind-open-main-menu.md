---
title: 停用按鍵綁定「Super_L」開啟「Main Menu」
nav_order: 7022
has_children: false
parent: 如何
---


# 停用按鍵綁定「Super_L」開啟「Main Menu」




## 參考文章

* Arch Wiki / KDE / [Disable opening application launcher with Super key (Windows key)](https://wiki.archlinux.org/title/KDE#Disable_opening_application_launcher_with_Super_key_(Windows_key))




## 設定檔

| 設定檔路徑 |
| --- |
| [~/.config/kwinrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kwinrc#L43-L44) |




## 設定片段

> 從原來的

``` ini
[ModifierOnlyShortcuts]
Meta=org.kde.plasmashell,/PlasmaShell,org.kde.PlasmaShell,activateLauncherMenu
```

> 改成如下

``` ini
[ModifierOnlyShortcuts]
Meta=
```




## 操作指令

執行下面指令，先把「plasma-kglobalaccel.service」停掉。

``` sh
systemctl --user stop plasma-kglobalaccel.service
```

執行下面指令，設定「~/.config/kwinrc」。

``` sh
kwriteconfig6 --file kwinrc --group ModifierOnlyShortcuts --key Meta ""
```

執行下面指令，接著把「plasma-kglobalaccel.service」啟動。

``` sh
systemctl --user start plasma-kglobalaccel.service
```




## 指定新的按鍵綁定

綁定「`Alt + F1`」或是「`Win + Space`」觸發「Main Menu」，

編輯「`~/.config/kglobalshortcutsrc`」。


> 舊版：[設定片段](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L270)

```
[plasmashell]
activate widget 3=Alt+F1\tMeta+Space,none,Activate Application Launcher Widget
```


> 新版：[設定片段](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L259) (6.2)

```
[plasmashell]
activate application launcher=Alt+F1\tMeta+Space,Meta\tAlt+F1,Activate Application Launcher
```


> 關於「舊版」的「`activate widget 3=`」是根據「[~/.config/plasma-org.kde.plasma.desktop-appletsrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/plasma-org.kde.plasma.desktop-appletsrc#L68-L87)」

```

[Containments][2][Applets][3]
immutability=1
plugin=org.kde.plasma.kickoff


[Containments][2][Applets][3][Configuration][Shortcuts]
global=Alt+F1

[Containments][2][Applets][3][Shortcuts]
global=Alt+F1

```




## 相關議題

| 相關議題 |
| ------- |
| [設定「Mouse Button Modifier」](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/howto/config-mouse-button-modifier.html) |
