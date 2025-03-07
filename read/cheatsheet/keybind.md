---
title: 鍵盤按鍵綁定一覽表
nav_order: 9010
has_children: false
parent: 一覽表
---


# 鍵盤按鍵綁定一覽表




## 主題

* [系統操作](#系統操作)
* [開啟應用程式](#開啟應用程式)
* [視窗操作](#視窗操作)
* [切換](#切換)
* [相關連結](#相關連結)




## 設定檔

> 關於「按鍵綁定」的設定檔

| 設定檔 |
| ----- |
| [~/.config/kglobalshortcutsrc](https://github.com/samwhelp/manjaro-kde-plasma-adjustment/blob/main/prototype/main/kde-config/locale/en_us/Breeze-Dark/asset/overlay/etc/skel/.config/kglobalshortcutsrc#L51) |




## 系統操作


## 系統操作 / 離開系統

| 按鍵組合           | 功能                   | 設定項目         |
| ------------------ | ---------------------- | ---------------- |
| `Alt + Shift + z`  | 鎖住                   | `Lock Session=`  |
| `Alt + Shift + x`  | 離開選單 (登出或關機)  | `Log Out=`       |




## 開啟應用程式


## 開啟應用程式 / 透過「應用程式啟動器」

| 按鍵組合    | 功能                                     | 設定項目                          |
| ----------- | ---------------------------------------- | --------------------------------- |
| `Alt + F1`  | `開啟「應用程式啟動主選單(Main Menu)」`  | `activate application launcher=`  |
| `Alt + F2`  | `開啟「應用程式啟動器(Runner)」`         | `krunner`                         |




## 開啟應用程式 / 透過「Rofi」

| 按鍵組合           | 功能                            | 執行指令                         |
| ------------------ | ------------------------------- | -------------------------------- |
| `Alt + Shift + d`  | 開啟 Rofi (可用應用程式列表)    | `rofi -show drun -show-icons`    |
| `Alt + Shift + w`  | 開啟 Rofi (已經開啟的視窗列表)  | `rofi -show window -show-icons`  |
| `Alt + Shift + r`  | 開啟 Rofi (可用指令列表)        | `rofi -show run`                 |




## 開啟應用程式 / Terminal

| 按鍵組合           | 功能           | 執行指令   |
| ------------------ | -------------- | ---------- |
| `Alt + Enter`      | 開啟 Terminal  | `konsole`  |
| `Alt + Shift + a`  | 開啟 Terminal  | `konsole`  |
| `Alt + Ctrl + a`   | 開啟 Terminal  | `sakura`   |
| `Alt + Shift + t`  | 開啟 Terminal  | `konsole`  |
| `Alt + Ctrl + t`   | 開啟 Terminal  | `sakura`   |


| 按鍵組合           | 功能                     | 執行指令   |
| ------------------ | ------------------------ | ---------- |
| `Alt + Shift + y`  | 開啟 Drop Down Terminal  | `yakuake`  |




## 開啟應用程式 / 常用的應用程式

| 按鍵組合           | 功能            | 執行指令          |
| ------------------ | --------------- | ----------------- |
| `Alt + Shift + f`  | 開啟檔案管理器  | `dolphin`         |
| `Alt + Shift + g`  | 開啟檔案管理器  | `pcmanfm-qt`      |
| `Alt + Shift + e`  | 開啟文字編輯器  | `kate`            |
| `Alt + Shift + b`  | 開啟網頁瀏覽器  | `firefox`         |
| `Alt + Shift + s`  | 開啟系統設定    | `systemsettings`  |




## 視窗操作

| 按鍵組合       | 功能                               | 設定項目                       |
| -------------- | ---------------------------------- | ------------------------------ |
| `Alt + Space`  | 顯示「視窗功能選單」               | `Window Operations Menu=`      |
| `Win + q`      | 關閉視窗                           | `Window Close=`                |
| `Win + f`      | 視窗全螢幕                         | `Window Fullscreen=`           |
| `Win + w`      | 視窗最大化                         | `Window Maximize=`             |
| `Win + x`      | 視窗最小化                         | `Window Minimize=`             |
| `Win + d`      | 切換「顯示桌面」                   | `Show Desktop=`                |
| `Win + e`      | 開始「視窗移動」                   | `Window Move=`                 |
| `Win + r`      | 開始「視窗更改大小」               | `Window Resize=`               |
| `Win + t`      | 視窗保持永遠在最上方               | `Window Above Other Windows=`  |
| `Win + b`      | 視窗保持永遠在最下方               | `Window Below Other Windows=`  |
| `Win + y`      | 視窗內容區塊收合                   | `Window Shade=`                |
| `Win + n`      | 切換顯示隱藏視窗裝飾(Decorations)  | `Window No Border=`            |
| `Win + z`      | 將下方視窗移上來                   | `Toggle Window Raise/Lower=`   |
| `Win + m`      | 視窗移動至畫面中央部位             | `Window Move Center`           |
| `Win + ;`      | 視窗更加透明                       | `Decrease Opacity=`            |
| `Win + '`      | 視窗更不透明                       | `Increase Opacity=`            |


> 一般預設「`Alt + F4`」綁定「`視窗關閉`」

> 一般預設「`F11`」綁定「`視窗全螢幕`」




## 切換

## 切換 / 視窗

| 按鍵組合     | 功能                        | 設定項目                                       |
| ------------ | --------------------------- | ---------------------------------------------- |
| `Win + a`    | 聚焦切換到「前面一個視窗」  | `Walk Through Windows (Reverse)=`              |
| `Win + s`    | 聚焦切換到「後面一個視窗」  | `Walk Through Windows=`                        |
| `Win + Esc`  | 聚焦切換到「前面一個視窗」  | `Walk Through Windows Alternative=`            |
| `Alt + Esc`  | 聚焦切換到「後面一個視窗」  | `Walk Through Windows Alternative (Reverse)=`  |

> 一般預設「`Alt + Tab`」綁定「`視窗聚焦切換`」




## 切換 / 工作空間

| 按鍵組合   | 功能                      | 設定項目                            |
| ---------- | ------------------------- | ----------------------------------- |
| `Alt + a`  | 切換到「上一個工作空間」  | `Switch One Desktop to the Left=`   |
| `Alt + s`  | 切換到「下一個工作空間」  | `Switch One Desktop to the Right=`  |




## 切換 / 概覽

| 按鍵組合       | 功能                        | 設定項目     |
| -------------- | --------------------------- | ------------ |
| `Win + grave`  | 切換到「所有工作空間概覽」  | `Overview=`  |
| `Win + Tab`    | 切換到「所有視窗概覽」      | `Expose=`    |

> 關於「grave」指是「`」，在「Tab鍵」上方的那個「鍵盤按鍵」。




## 相關連結

| 相關連結 |
| ------- |
| [鍵盤按鍵綁定](https://samwhelp.github.io/note-about-manjaro-kde-plasma/read/config/keybind.html) |
