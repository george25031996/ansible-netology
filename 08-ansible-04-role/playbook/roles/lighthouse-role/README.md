Role Name
=========

Роль для установки lighthouse.

- Установка Git
- Скачивание lighthouse из репозитория
-Конфигурирование lighthouse


Requirements
------------

- Должен быть установлен git. Если его нет, роль произведёт его установку
- Требуется отдельная установка и настройка Nginx

Role Variables
--------------

Переменные для установки default/main.yml:

clickhouse_user: glisikh
clickhouse_password: glisikh

Переменные для скачивания lighthouse из git и конфигурационных файлов lighthouse/nginx vars/main.yml

lighthouse_vcs: https://github.com/VKCOM/lighthouse.git
lighthouse_dir: /var/lib/lighthouse
lighthouse_access_log_name: lighthouse_access

Dependencies
------------

Требуется роль clickhouse-role

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

hosts: lighthouse
roles:
  - role: lighthouse-role

License
-------

MIT

Author Information
------------------

