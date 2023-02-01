
# CKANのデータを可視化する(CKANからGOOGLE Looker Studioへの連携)

この研修ではCKANに登録されたオープンデータをGOOGLE Looker Studioで可視化する事を目的とします。
CKANに登録されたデータを直接GOOGLE Looker Studioに取り込むことはできないので、
CKANのオープンデータをGOOGLE Spread Sheetに入れてそのGOOGLE Spread SheetをGOOGLE Looker Studioにて可視化します。
 
 ## 1. Google Spread Sheet のアドイン導入<br>
CKANのデータをGOOGLE Spread Sheetに取り込む方法はいくつかあります。
・GOOGLE Spread Sheetの機能拡張アドオンを利用する
・GASプログラムを作成する
・GASプログラムのサンプルを利用する

この研修ではGOOGLE Spread Sheetの機能拡張アドオンを利用することとします。

### Spread Sheetの機能拡張アドオン　API Connector を追加する<br>
```
機能拡張メニュー=>アドオン=>アドオンを取得　
```
を選択します。
検索欄に　「API Connector」と入力し
API Connector　を探します。（白地に青い文字）
API Connector　を選択します。

２つあるボタンの下の方
```
「個別インストール」
```
をクリックします。
**ワンポイントアドバイス**<br>
1つめのボタンを押すとアドオンをインストールする組織の範囲を決める事ができます。
```
次のユーザーにアプリを自動インストールする
 組織内の全ユーザー
 特定のグループまたは組織部門
```
### API Connector を設定する <br>
```
機能拡張メニュー=>API Connector=>open　を選択します。
```
Request タブの中の　Create Request を選択します。<br>

２つ目の
```
Request URL
```
の箇所を変更します。
```
https://data.bodik.jp/api/3/action/datastore_search_sql?sql=SELECT%20*%20from%20%225f21adb5-9eba-4e2f-b7aa-d6aa8ad05e02%22
```
と入力します。



#CKANのデータを可視化する

##


参考ページ
飯塚市オープンデータ
https://lookerstudio.google.com/reporting/56063a64-0e44-4e75-a81d-082a9f2807ef/page/p_cnea439p1c
データで見るBODIK
https://lookerstudio.google.com/reporting/341f7ea6-38a8-43ac-8483-9b66c0f085b6/page/p_g29wqs41wc
聞きたい事
使用したいデータ、CSV、見方があれば教えて頂きたい。
使用したデータ（那覇市　地域・年齢別人口　令和4年12月末時点）
https://www.city.naha.okinawa.jp/online/opendata/jinkou/open202212.html
APIの元　沖縄県医療機関一覧（令和４年10月31日時点）
https://data.bodik.jp/api/3/action/datastore_search_sql?sql=SELECT%20*%20from%20%225f21adb5-9eba-4e2f-b7aa-d6aa8ad05e02%22 （編集済み） 

 
　リアルタイム性の確認
　データ項目の準備
　可視化　例（人口ピラミッド）
　地図の可視化の例
　ジオコーダー
　IPからロケーションへサンプル
