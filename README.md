# Laravel 11 Streply 錯誤紀錄

引入 streply 的 streply-laravel 套件來擴增使用 Streply 管理錯誤和日誌、評估活動並提高效能，它不僅自己捕捉所有錯誤，而且還將錯誤發送到 Streply 的資料庫，這種方法不僅速度快，而且非常方便。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。

## 畫面截圖
![](https://i.imgur.com/03YuQNj.png)
> 觸發錯誤例外以中斷程式流程

![](https://i.imgur.com/paMTBaz.png)
> 使用 Streply 確認程式錯誤的偵測
