Настройка nginx + php5-fpm + mysql с помощью Ansible.

Тестировалось только на Ubuntu 12.04!

Запуск:

ansible-playbook -i inventory.ini -u root playbooks/playbook.yml

Так как некоторые функции не реализованы, то после установке выполните:

1. adduser playrix
2. adduser playrix sudo
3. sudo chmod +x /root/iptables
4. addgroup sftp
5. adduser deploy
6. adduser deploy sftp
7. usermod -d /var/www/s1 deploy

Finish!