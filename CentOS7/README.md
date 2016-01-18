# CentOS7の場合

## JDKをインストール
 * 場所は/usr/java
 * JAVA_HOMEを定義し、PATHに$JAVA_HOME/binを追加する


## Tomcatをインストール
 * tar.gzを解答するだけ
 * 場所は/opt/tomcatにする
 * port8080をあける
  * firewall-cmd --permanent --add-port=8080/tcp
  * firewall-cmd --reload

## gitbucketをデプロイ
 * ダウンロードしたgitbucket.warを/opt/tomcat/apache～/webapp配下に転送
 * tomcatを起動する

## jenkinsインストール
 * yumまたはrpmでインストール
 * ポートを解放（手順は上記Tomcat記述参照）

