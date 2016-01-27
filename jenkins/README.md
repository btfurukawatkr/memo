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

## change port number
 * defalt port(8080,8009) number is already used by tomcat

## add plugins
 ### download and add to /var/lib/jenkins/plugin
 * git-plugin
 * scm-api
 * git-client

## jenkins plugins to install
 * git
 * ghprb
 * github
 * github-api
 * token-macro
 * plain-credentials
 * ssh-agent
 * workflow-step-api
 * workflow-aggregator
 * credentials

