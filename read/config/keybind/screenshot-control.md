---
title: 螢幕截圖
nav_order: 5054
has_children: false
parent: 按鍵綁定
grand_parent: 設定
---


# 螢幕截圖

> KDE Plasma Adjustment / [Keybind](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/tree/main/prototype/main/demo-config/keybind/demo-keybind-mode-dolphin)


* [設定片段](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L226-L234)

| 按鍵組合          | 功能             | 執行指令                                    |
| ----------------- | ---------------- | ------------------------------------------- |
| `Alt + Print` | 螢幕截圖(開啟Spectacle)         |  |
| `Win + Print` | 螢幕截圖(目前聚焦的視窗)         | `ActiveWindowScreenShot=` |
| `Print` | 螢幕截圖(目前桌面)         | `FullScreenScreenShot=` |
| `Ctrl + Print` | 螢幕截圖(選取區塊)         | `RectangularRegionScreenShot=` |
| `Shift + Print` | 螢幕截圖(滑鼠游標當下的視窗)         | `WindowUnderCursorScreenShot=` |


* [Spectacle](https://apps.kde.org/spectacle/) ([中文](https://apps.kde.org/zh-tw/spectacle/))
