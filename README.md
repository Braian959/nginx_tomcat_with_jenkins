Playbook запускается на localhost (внесён в inventory)
# Для работы proxy pass
Перед запуском необходимо вписать IP адрес вирт. машины в nginx.conf в строчку proxy_pass перед портом :8080
# Файл jenkins.war находится в корне репозитория

# После развёртывания jenkins будет доступен по http://IP:8080/jenkins
# Пароль для инициализации jenkins можно посмотреть, выполнив на хосте, где запущен контейнер, команду: 
docker exec -it tomcat cat /root/.jenkins/secrets/initialAdminPassword


# Proxy для jenkins настроить НЕ ПОЛУЧИЛОСЬ, для tomcat PROXY работает!
