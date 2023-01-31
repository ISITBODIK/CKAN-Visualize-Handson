
# docker, docker-compose

## 1. gitを使えるようにする<br>
```
sudo yum update -y
sudo yum install -y git
```
ハンズオンの資料を取り寄せる
```
mkdir handson
cd handson
git clone https://github.com/ISITBODIK/CKAN-Install-Handson.git .
```
## 2. dockerを使えるようにする<br>
```
cd shell
./docker.sh
cd ..
```
## 3. nginxを動かしてみよう
```
docker run --name some-nginx -d -p 80:80 nginx
```
## 4. docker-composeでnginxを動かしてみよう<br>

#CKANのデータを可視化する

##

CKANからGOOGLE　Looker Studioへの連携
　（GOOGLE Spread Sheet を介して）
　Google Spread Sheet のアドイン導入
　リアルタイム性の確認
　データ項目の準備
　可視化　例（人口ピラミッド）
　地図の可視化の例
　ジオコーダー
　IPからロケーションへサンプル
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


