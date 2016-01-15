# Tomcatをインストール
 * Apacheのサイトからapache-tomcat-xxx.tar.gzをダウンロードしてサーバに転送
 * 場所は/opt/tomcatにする
 * tar xvzf apache-tomcat-xxx.tar.gz
 * port8080をあける
  * firewall-cmd --permanent --add-port=8080/tcp
  * firewall-cmd --reload


