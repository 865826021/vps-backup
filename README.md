# VPS数据备份及数据库备份

支持轮询备份

备份数据如下
/home/wwwroot目录下所有站点目录（支持init配置备份目录），排除phpMyadmin
mysql全部数据库（排除的表：mysql、performance_schema、information_schema）
/usr/local/nginx/conf/vhost 全部文件

支持一键恢复
./backup.sh Restore

Usage: ./backup.sh init|backup|db|Restore
