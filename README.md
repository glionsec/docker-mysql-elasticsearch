# docker-ELK-DB

Docker上でelasticstack(elasticsearch,kibana,logstash)とmysql(phpmyadmin含む)を連携させて稼働させる。

細かい部分は現在調整中


.env_mysqlが消えてしまうのでここに記載

  MYSQL_DATABASE=change_me

  MYSQL_USER=change_me

  MYSQL_PASSWORD=change_me

  MYSQL_ROOT_PASSWORD=change_me


接続先：

  kibana：5601

  elasticsearch：9200

  logstash：5000

  mysql：3306

  phpmyadmin：3000


起動前に必要なコマンド：

  chmod a+x ./init/*.sh

  docker volume create elasticstack

  docker volume ls

  docker network create elasticstack

  docker network ls

起動：

  docker-compose up -d

終了：

  docker-compose down


参照先：

  https://qiita.com/kenchan1193/items/9320390d48f3d2ae883c

  https://zenn.dev/ajapa/articles/938499b8c96926

  https://zenn.dev/jojojo/articles/f1223bb06cf5be

  https://qiita.com/k_ken/items/78c7a120de91516b2a09

  https://paltee.net/archives/911
