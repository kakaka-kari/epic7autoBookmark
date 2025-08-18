# epic7autoBookmark

第七史詩刷商店的小工具

![image](https://github.com/steven010116/epic7autoBookmark/assets/24381832/526e78b9-df97-4500-9758-55f514eed883)

目前這個版本不支援國服，如果有國服的使用需求可以參考這位大佬維護的專案 [epic7auto](https://github.com/Wrong-pixel/epic7auto)

## 零、前言

本程式由[steven010116](https://github.com/steven010116)大佬開發，本人只是做後續更新
大佬的Repository: [epic7autoBookmark](https://github.com/steven010116/epic7autoBookmark)

## 一、環境

0. windows10
1. Bluestacki. 版本：理論上全版本通用ii. 顯示：橫向、1920x1080、240DPI or 320DPI
2. ~~第七史詩i. 裝置詳細設定和遊戲詳細設定最好都不勾，如果覺得畫面太醜，高畫質套件測試過也是能正常運行ii. 推薦：只勾高級設定~~
   2025/4/21更: 現在好像沒有高畫質套件了，特殊效果開啟/關閉應該都可以執行。 (Raven9527)
3. python3.9.10
4. config.json
   ![預覽](https://i.imgur.com/2sAobaw.png)
   i. adb_addr填adb路徑
   ii. e7_language填e7裡的語系(繁中: zh-TW, 簡中: zh-CN, 英文: en-US)

## 二、使用方式

先將bluestack和第七史詩的設定調整的如上方環境相同。
adb功能在設定=>進階=>Android調試橋(ADB)，勾選後會看到路徑。
英文路徑在settings=>Advanced=>Android Debug Bridge(ADB)。

![預覽](https://i.imgur.com/eSamCR3.png)

確認第七史詩語系是不是與config.json裡使用的相同(預設為繁中)。

0. 綠色按鈕code > download zip 整包下載後解壓縮放在同一個資料夾下，路徑最好為英數避免有其他問題。
1. 參考上面的環境，確認config.json內的參數都是對的。
2. 開啟遊戲，進到秘密商店後，畫面會長得像下面這樣。

![預覽](https://i.imgur.com/KxeSpWM.png)

3. 打開小工具(main.exe)，選擇條件並輸入目標次數，按下開始應該就會自己動惹。
4. 之前的版本用圖像辨識，而這個版本走的是android adb，已經不會搶滑鼠了，甚至可以縮小放著。
5. .exe是用pyinstaller包的，有安全疑慮的話可以自己打包 `pyinstaller -F -w -i main.ico main.py`。

## 三、貢獻者
- [steven010116](https://github.com/steven010116) - 原作者
- [kakaka-kari](https://github.com/kakaka-kari) - 手動提前結束時，也產生結算報告

### 四、更新履歷
##### 2025/4/21: 第六史詩改版:
1. 對應UI更新，更新辨識之圖片 (目前僅繁中版圖片)
2. 對應聖域移除，移除自動點擊派遣功能

##### 2025/7/10: 湖畔魔女泰妮布里雅改版
1. 調整辨識程度 (官方可能微調UI導致辨識不到購買書籤的按鈕，因此做出調整)

#### 2025/8/19: 七周年紀念Part2改版:
1. 手動提前結束時，也產生結算報告 (特別感謝[kakaka-kari](https://github.com/kakaka-kari))
