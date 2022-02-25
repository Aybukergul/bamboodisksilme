# bamboodisksilme


df -kh ile verilere bakıldı
/dev/mapper/centos-root  altındaki doluluktan sonra; tüm image silindi

nexus a image atılmama sebebyidi.
 crontab -e
ile girildi
0 3 * * * docker rmi -f $(docker images -aq)
eklendi 

00:30 da tüm imageleri sil komutu 

ps -ef | grep nexus
 ile nexus nerede çalışıyor bulundu
 
  crontab -l
ile kontrol 
