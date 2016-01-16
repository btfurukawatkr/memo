# jenkins
## install by yum
 * wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo
 * rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
 * yum install jenkins

## keystore
 * cd /var/lib/jenkins
 * mkdir .ssl
 * keytool -genkey -alias jenkins-ssl-cert -keyalg RSA -keystore .ssl/keystore.jks -storepass Password01!

## jenkins sysconfig
 * vi /etc/sysconfig/jenkins
 * JENKINS_HTTPS_KEYSTORE="/var/lib/jenkins/.ssl/.keystore"
 * JENKINS_HTTPS_KEYSTORE_PASSWORD="Password01!"

## changge port number
 * defalt port number is already used by tomcat
