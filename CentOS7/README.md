# CentOS7�̏ꍇ

## JDK���C���X�g�[��
 * �ꏊ��/usr/java
 * JAVA_HOME���`���APATH��$JAVA_HOME/bin��ǉ�����


## Tomcat���C���X�g�[��
 * tar.gz���𓚂��邾��
 * �ꏊ��/opt/tomcat�ɂ���
 * port8080��������
  * firewall-cmd --permanent --add-port=8080/tcp
  * firewall-cmd --reload

## gitbucket���f�v���C
 * �_�E�����[�h����gitbucket.war��/opt/tomcat/apache�`/webapp�z���ɓ]��
 * tomcat���N������

## jenkins�C���X�g�[��
 * yum�܂���rpm�ŃC���X�g�[��
 * �|�[�g������i�菇�͏�LTomcat�L�q�Q�Ɓj

