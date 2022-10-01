# Facebook-Screenshot
此專案利用爬蟲概念爬取指定Facebook頁面前3個文章，並產生出該文章之截圖畫面。


因Facebook之CSS Class為動態產生，因此會因為Class的更新導致無法爬取正確資料。
本專案使用相對路徑之爬蟲方式解決了本問題，因此Class的更新並不會導致本專案無法使用。

## 需求
- Python >= 3.9
- ChromeDriver

## 使用方式

1. 從 [ChromeDriver - WebDriver for Chrome](https://chromedriver.chromium.org/downloads) 下載支援自身Chrome的版本。
2. 放置 chromedriver 至預設位置 `C:/chromedriver_win32/chromedriver.exe` (可於`main.py`中修改)。
3. 開啟 `main.py` 並修改 `FB_ACCOUNT`, `FB_PASSWORD` 成自身Facebook之帳號密碼。
4. 開啟 `pages.txt` 並新增/刪除所需要的Facebook頁面
5. 安裝執行所需套件執行指令 ``` pip3 -r requirements.txt ```

以上步驟執行完成後執行以下指令

```
python3 main.py
```

## DEMO

以 `pages.txt` 中的Facebook頁面連結為例子之輸出可參考 `2022_10_01-11_03_17_AM.docx`
