# mysqlTutorial

sudo yum install https://dev.mysql.com/get/mysql80-community-release-el7-3.noarch.rpm // 「.rpm」ファイルは、Linux用に開発されたパッケージ形式.  
sudo rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022 // 鍵のエラー解決するやつ.  
sudo systemctl start mysqld //.  
sudo systemctl enable mysqld //.  
systemctl status mysqld // MySQLの状態確認.  
sudo grep 'temporary password' /var/log/mysqld.log // 一時的なパスワードを表示。grepはファイル中の文字列を検索するコマンド.   
mysql -u root -p // mysqlに一時的なパスワードでログイン.  
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'MyNewPass1!'; // 新しいパスワードを設定.  
mysql -u root -p //　新しいパスワードでログイン.   


