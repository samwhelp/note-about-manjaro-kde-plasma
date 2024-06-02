---
title: 設定「Mouse Button Modifier」
nav_order: 7021
has_children: false
parent: 如何
---


# 設定「Mouse Button Modifier」




## 期望功能

我個人習慣「[在視窗操作下面兩個動作](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/config/mousebind.html#視窗內容區塊)」，

| 滑鼠按鍵組合                |  功能                   |
| --------------------------- | ----------------------- |
| `Win + [滑鼠左鍵按住拖曳]`  | 視窗移動                |
| `Win + [滑鼠右鍵按住拖曳]`  | 視窗更改大小            |




## 設定檔

| 設定檔路徑 |
| --- |
| [~/.config/kwinrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kwinrc#L46-L47) |




## 圖形介面操作

開啟「System Settings」，

在「System Settings / Window Management / Window Behavior / Window Actions」這個頁面，

有一個設定區塊「Inner Window, Titlebar and Frame Actions」，


其中有一個設定「`Modifier Key:`」，下拉選單的選項如下

| 選項  |
| ---- |
| `Meta` |
| `Alt`  |

這個設定的「預設值」是「`Meta`」。

若是將「設定值」改成「`Alt`」，按下「Apply」這個按鈕，

這個「設定值」會被儲存在「[~/.config/kwinrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kwinrc#L46-L47)」這個檔案。

設定片段如下：

``` ini
[MouseBindings]
CommandAllKey=Alt
```

若是將「設定值」改成「`Meta`」，按下「Apply」這個按鈕，

則「`CommandAllKey=Alt`」那一行就會被刪除，也就是預設是「`Meta`」。



我們也可以手動修改「[~/.config/kwinrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kwinrc#L46-L47)」這個檔案。

將「設定值」改成「`Meta`」，設定片段如下：

``` ini
[MouseBindings]
CommandAllKey=Meta
```




## 搭配設定

在設定區塊「Inner Window, Titlebar and Frame Actions」，

除了「`Modifier Key:`」這個設定，還有下面幾個搭配的設定：

| 搭配設定           | 預設值                    ｜
| ---------------- | ------------------------- |
| `Left click:`    | `Move`                    |
| `Middle click:`  | `Toggle raise and lower`  |
| `Right click:`   | `Resize`                  |
| `Mouse wheel:`   | `Change opacity`          |




## 相關設定

另外因為我慣用「Win鍵」的「按鍵組合」來操作一些「視窗動作」，

例如「`Win + q` => 視窗關閉」，「`Win + m` => 視窗最大化」。

預設按下「Win鍵」會觸發「顯示Menu」，

為了避免無謂的干擾，我會停用這個功能，

請參考『[停用按鍵綁定「Super_L」開啟「Main Menu」](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/howto/disable-keybind-open-main-menu.html)』這篇的說明。




## 相關議題

| 相關議題 |
| ------- |
| [滑鼠按鍵綁定](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/config/mousebind.html#視窗內容區塊) |
| [停用按鍵綁定「Super_L」開啟「Main Menu」](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/howto/disable-keybind-open-main-menu.html) |




## 相關應用

* Menu Applet 開發筆記 / [demo-mouse-button-modifier](https://samwhelp.github.io/note-about-menu-applet/read/demo/demo-mouse-button-modifier.html#cinnamon)
