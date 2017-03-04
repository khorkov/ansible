Настройка nginx + php5-fpm + mysql с помощью Ansible.

Тестировалось только на Ubuntu 12.04!

Создаем ключи и запускаем агента.

1. ssh-keygen
2. eval "$(ssh-agent -s)"
2. ssh-add ~/.ssh/id_rsa

Запуск:

ansible-playbook -i inventory.ini config/provision/playbook.yml

Finish!