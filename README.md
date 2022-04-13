# 待辦事項管理清單(To-do List)
此待辦事項管理清單(To-do List)是一個待辦事項管理工具，可讓使用者新增、瀏覽、修改與刪除待辦事項

## 專案畫面
![register](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/register.png)
![login](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/login.png)
![Index](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/index.png)
![New](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/new.png)
![Edit](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/edit.png)
![Detail](https://github.com/aziz0916/todo-sequelize/blob/main/public/images/detail.png)

## 專案功能
1. 使用者可以註冊帳號
   + 註冊之後，可以登入/登出
   + 只有登入狀態的使用者可以看到app內容，否則一律被導向登入頁
2. 使用者可以在首頁一次瀏覽所有待辦事項
   + 使用者只能看到自己建立的資料
3. 使用者可以新增一筆待辦事項
4. 使用者可以修改待辦事項
5. 使用者可以刪除任何一筆待辦事項

## 使用工具
- [Visual Studio Code](https://visualstudio.microsoft.com/zh-hant/) 1.66.0 - 開發環境
- [Express](https://www.npmjs.com/package/express) 4.17.1 - 應用程式架構
- [Express-Handlebars](https://www.npmjs.com/package/express-handlebars) 4.0.4 - 模板引擎
- [MySQL](https://www.mysql.com/) 8.0.15 - 資料庫
- [mysql2](https://www.npmjs.com/package/mysql2) 2.1.0 - 讓Node.js能使用MySQL的套件
- [Sequelize](https://www.npmjs.com/package/sequelize) 5.21.13 - MySQL 的 ORM 可以在程式中與資料庫溝通
- [sequelize-cli](https://www.npmjs.com/package/sequelize-cli) 5.5.1 - 提供了一系列好用的終端指令
- [method-override](https://www.npmjs.com/package/method-override) 3.0.0 - 增加除瀏覽器自帶的GET與POST以外的偽請求，增加介面語義化
- [express-session](https://www.npmjs.com/package/express-session) 1.17.1 - 儲存認證結果
- [Passport](https://www.npmjs.com/package/passport) 0.4.1 - 認證使用者
- [passport-local](https://www.npmjs.com/package/passport-local) 1.0.0 - 使用username和password方式進行身分驗證
- [passport-facebook](https://www.npmjs.com/package/passport-facebook) 3.0.0 - 通過Facebook進行身份驗證
- [connect-flash](https://www.npmjs.com/package/connect-flash) 0.1.1 - 製作系統訊息功能
- [bcrypt.js](https://www.npmjs.com/package/bcryptjs) 2.4.3 - 進行雜湊加密
- [dotenv](https://www.npmjs.com/package/dotenv) 8.2.0 - 將敏感資訊寫入環境變數

## 安裝
1. 開啟終端機(Terminal)，Clone 此專案至本機電腦

```
git clone https://github.com/aziz0916/todo-sequelize.git
```
2. 進入存放此專案的資料夾

```
cd todo-sequelize
```
3. 安裝 npm 套件

```
npm install
```
4. 將 .env.example 檔案名改成 .env，並將檔案中 SKIP 相關參數進行更改。
5. 引入種子資料

```
npx sequelize db:seed:all
```
6. 測試種子資料

| Name | Email | Password |
| ------------- | :---: | -------- |
| root          | root@example.com| 12345678  |
7. 執行程式

```
npm run dev
```
