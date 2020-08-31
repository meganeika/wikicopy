Docker開発検証環境
構築手順

![docker開発検証環境構築手順_page-0001](uploads/94263f5e3ca9a5f0e03e5e1eb727e084/docker開発検証環境構築手順_page-0001.jpg)


l.dockerをローカルに
インストール

・方法は各自の環境に適した手順をググってください。

![docker開発検証環境構築手順_page-0002](uploads/f8aea70eeb66856b8f8a0d48f5a12c37/docker開発検証環境構築手順_page-0002.jpg)


2."

dockerlogin

"コマンドで
Dockerhubにログイン



・実行するディレクトリはどこでも大丈夫です。

![docker開発検証環境構築手順_page-0003](uploads/bb389321ab7fd16ad9db4fc652c73842/docker開発検証環境構築手順_page-0003.jpg)



3."

docker pull hackathonIite2020/django:var1.0

コマンドでDockerイメージを取得

![docker開発検証環境構築手順_page-0004](uploads/af49e4b52ac8df83a28774dc33066bdf/docker開発検証環境構築手順_page-0004.jpg)



4."

docker images

"コマンドで「django」
のイメージが取得できている事を確認

![docker開発検証環境構築手順_page-0005](uploads/e55945d1d4f6bb975609bc851ee094e3/docker開発検証環境構築手順_page-0005.jpg)





5."docker run -itd -p 8000:8000 -v 

<各自ローカルの「mimamorukun」ティレクトリまでのフルバス>

:/code--name django-dev hackathonlite2020/django:var1.O

"
コマンドでコンテナ起動


"

docker ps

"コマンドでコンテナが立ち上がっている事を
確認してください。

![docker開発検証環境構築手順_page-0006](uploads/f997e758bcf368c4f0110aa16a81c4c1/docker開発検証環境構築手順_page-0006.jpg)


6."

docker exec django-dev python3 manage.py runserver 0.0.0.0:8000

"コマン
ドでサーバ立ち上げ




![docker開発検証環境構築手順_page-0007](uploads/d5707f5290f72d05f23c7659d56c6c46/docker開発検証環境構築手順_page-0007.jpg)


7."http://locaIhost:8000/< 確 認 し た い パ ス > " で ブ ラ ウ ザ か ら 参 照 で き る 事 を 確 認 


・ 山 下 さ ん 作 成 の プ ロ ト タ イ プ を ロ ー カ ル に ダ ウ ン ロ ー ド し て 表 示 し て い ま す 。 

コ ン テ ナ 内 に Django が 入 っ て い る の で 、 ロ ー カ ル に jdango が イ ン ス ト ー ル さ 
れ て な く て も 画 面 表 示 で き て い ま す 。 


![docker開発検証環境構築手順_page-0008](uploads/d841051957217b112553ed3458ce7825/docker開発検証環境構築手順_page-0008.jpg)


![docker開発検証環境構築手順_page-0009](uploads/65d2b7f9c83770bd0ec0b5d65f359699/docker開発検証環境構築手順_page-0009.jpg)

















