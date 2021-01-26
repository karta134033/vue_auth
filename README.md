# Vue簡易登入搭配token機制
後端需要搭配"django_auth"的專案

## 所需套件
* md5加密: 
  npm install js-md5 --save-dev
* axios: 
  npm install --save axios vue-axios
* vue-router: 
  npm install --save vue-router
* vuetify: 
  vue add vuetify 

開一個新專案的方式可以參考Vue官網。

## API請求與驗證

### 登入頁面
![](https://i.imgur.com/9b4XJBm.png)
* 起始頁面，帳號密碼需要在後端先設定好。
* 登入成功後會導轉到測試頁面。
* 登入失敗會跳出視窗告知。

### 測試頁面

* 檢查有沒有uid與token的資訊。
  ![](https://i.imgur.com/wvSbipS.png)
* group的資料需要先由POST方法塞入資訊。
* 塞入資訊後試著GET資料，看能不能取得資料庫內所有group的資訊。
  ![](https://i.imgur.com/0wDlXaL.png)


