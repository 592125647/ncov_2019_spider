
mongodb ���ڲɼ������ݿ����
��װ����for mac :https://www.runoob.com/mongodb/mongodb-osx-install.html
����mongo ������
mongod --dbpath d:/workspace/mongodb
export PATH=/usr/local/mongodb/bin:$PATH && sudo mongod

mysql ��װ
ж��mysql
sudo rm /usr/local/mysql
sudo rm -rf /usr/local/mysql*
sudo rm -rf /Library/StartupItems/MySQLCOM
sudo rm -rf /Library/PreferencePanes/My*
rm -rf ~/Library/PreferencePanes/My*
sudo rm -rf /Library/Receipts/mysql*
sudo rm -rf /Library/Receipts/MySQL*
sudo rm -rf /var/db/receipts/com.mysql.*

networksetup -setairportpower en0 off && networksetup -setairportpower en0 on


���� �� http://dev.mysql.com/get/Downloads/MySQL-5.7/mysql-5.7.10-osx10.9-x86_64.dmg
��װ������https://www.cnblogs.com/kimbo/p/8724595.html
root@localhost: 4O=ucCLx9y%3
/usr/local/mysql-5.7.10-osx10.9-x86_64/bin

��������
1. �ر�mysql����
sudo /usr/local/mysql/support-files/mysql.server stop ����ϵͳƫ�����и� MySQL ��ر�
2.����mysqlĿ¼��
/usr/local/mysql-5.7.10-osx10.9-x86_64/bin
3.�õ�Ȩ��
sudo su
4.����mysql����
./mysqld_safe --skip-grant-tables &? ������ϵͳ����п���
5.�ؿ��ն�
mysql -uroot -p ����ʾ��������ʱ������뼴��
6. �õ�Ȩ�ޣ������޸����룩
flush privileges;
7.�޸�����
set password for 'root'@'localhost'=password('root');
set password for 'root'@'localhost'=password('root');

 


��װnavicat
http://www.pc6.com/mac/111878.html
���նˣ����룺sudo spctl --master-disable �س�����ƫ�����õİ�ȫ������˽�������κ���Դ�����´�Navicat for MySQL��OK��


��װ������

python3 -m pip install -r requirements.txt


crawler.py ����������������ļ�
python crawler.py 
�����󣬾ͻ�ѭ���������ȡ����������⵽mongo

spider.py ��mongo 2 mysql ������ת����
��Ҫ�Ƿ������ʹ��sql �����ݲ�ѯ���о���
Ҳ��Ҫ����������ʵʱת�����ݵ�mysql
python spider.py


#��һ�����������ݿ�
sudo pkill mongod
export PATH=/usr/local/mongodb/bin:$PATH && sudo mongod
#�ڶ�������������ת����mongo 2 mysql��
cd /Users/HE/Desktop/ncov_spider/ && python3  spider.py
# ���������������棨ÿ�춼Ҫ���������������ػ��ͻ�һֱ��ÿ���Զ���
cd /Users/HE/Desktop/ncov_spider/ && python3  main.py 

����3�����������һ���µ��ն�ִ�С�

���ݿ����ƣ�ncov
��ѯʵ������ҵ��.sql

�� ��
dxyarea  ʡ������
dxyarea_city ���м�����


