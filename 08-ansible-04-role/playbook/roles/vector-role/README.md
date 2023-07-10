Role Name
=========

Роль для установки vector.

- Установка vector
- Создание systemd unit Vector
- Конфигурирование vector на передачу данных в clickhouse


Requirements
------------


Role Variables
--------------

Переменные для установки кредов default/main.yml:

clickhouse_user: glisikh
clickhouse_password: glisikh

Dependencies
------------

В inventory должен быть хост clickhouse-01

endpoint: ip-adress:8123

Требуется роль clickhouse-role

Example Playbook
----------------

hosts: vector
roles:
  - role: vector-role

License
-------

MIT

Author Information
------------------

