# Angular01 - Angular 介紹及環境建置

使用 Angular 作為前端開發框架四年多了，一直都覺得 Angular 的世界就像浩瀚宇宙一樣，永遠都有學習之處，也想更深入 Angular 底層結構的概念，並與這幾年所學習到的技巧、個人使用經驗，相互結合，也希望能幫助到讀者們快速進入 Angular 的世界。

[目錄]
- [Angular01 - Angular 介紹及環境建置](#angular01---angular-介紹及環境建置)
  - [Angular 是什麼](#angular-是什麼)
  - [開發環境建置](#開發環境建置)
    - [Angular CLI](#angular-cli)
      - [Angular CLI 常用指令](#angular-cli-常用指令)
      - [Angular 各版本兼容性](#angular-各版本兼容性)
  - [參考網站](#參考網站)


## Angular 是什麼
Angular 是基於 [TypeScript](https://www.typescriptlang.org/) 的建構客戶端應用的平臺與框架，主要用於開發大型專案。它包括：

- 一個基於元件的框架，用於建構可伸縮的 Web 應用
- 一組完美整合的函式庫，涵蓋各種功能，包括路由、表單管理、客戶端-伺服器通訊等
- 一套開發工具，可幫助你開發、建構、測試和更新程式碼

以上是官方所寫的介紹，簡單來說 Angular 是一個很強大的框架，在 Angular 中定義了許多概念，所以要學習也是需要一些時間。如果想要先快速要寫出一個小專案，可以先利用官方文件的[**快速教學**](https://angular.tw/start)了解 Angular 最基本的應用，再學習更深入的 Angular 框架。
另外， Angular 是基於 [TypeScript](https://www.typescriptlang.org/) 所建構的，也可以先查看 TypeScript 的程式寫法，有助於在 Angular 的路上越走越順。

> 官方網站: https://angular.io

## 開發環境建置

先安裝 [Node.js](https://nodejs.org/en/) 及 [npm 套件管理器](https://docs.npmjs.com/)。
LTS 是大多數人都在使用的版本；Current 則是目前最新的版本，選其中一個版本下載即可。
下載完成後，開啟終端機或命令提示字元，輸入 `node -v` 及 `npm -v` 確認是否安裝完成。

![](https://i.imgur.com/mktfovD.png)

接著下載 [Angular CLI](https://angular.tw/cli)
在終端機下輸入 `npm install -g @angular/cli` 下載 Angular CLI

### Angular CLI
Angular CLI 是 Angular 的命令列工具，提供了各種簡化作業的指令，讓使用者能快速進行 Angular 的開發，推薦建立新專案或文件時，可以利用 CLI 指令，避免有些地方沒有同步引用module，導致無法執行。

利用終端機移至選定好的資料夾，輸入下列指令:
```
ng new MyFirstAngular
```
接著會詢問是否需要自動增加 Angular routing 及選擇 stylesheet format
這些都由個人選擇就可以了，通常我會預設增加 routing 及選擇 scss format
![](https://i.imgur.com/1cYCv4Y.png)


接著移到該目錄的資料夾中並輸入下列指令：
```
cd MyFirstAngular
ng serve
```
即可在瀏覽器中開啟 http://localhost:4200/ 檢視執行效果。


**:bulb: tip**
Angular CLI 的版本會影響利用 CLI 建立新專案的 Angular 版本。
例如: Angular CLI 的版本若為10，建立出的 Angular 版本為10。


#### Angular CLI 常用指令

| 指令 | 說明 |
| -------- | -------- | 
|ng -help | 查詢 CLI 所有指令|
|ng v| Angular CLI 版本|
| ng new {專案名稱}| 建立新專案     | 
| ng serve| 啟動 Angular 應用程式|
| ng new generate(g) {Schematics} | 建立特定的元件，例如 `ng new g component`能建立 component。 |
|ng build {專案名稱} |程式編譯|

#### Angular 各版本兼容性
參考連結: https://gist.github.com/LayZeeDK/c822cc812f75bb07b7c55d07ba2719b3


## 參考網站
[Angular 官方文件](https://angular.tw/guide/what-is-angular)
[Angular 新手入門
](https://developer.mozilla.org/zh-TW/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Angular_getting_started)
