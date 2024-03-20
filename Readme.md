# Название
Плейбук TICK Stack

# Описание работы плайбука

1. Устанавливаем docker
2. Устанавливаем python и pip
3. Устанавливаем через pip-менеджер docker-compose
4. Клонируем репу *https://github.com/influxdata/sandbox/tree/master*
5. Запускаем *docker-compose.yml up* из директории в которую склонировали репу


# Требования к инсталляции плейбука

1. Дополнительно необходимо установить коллекцию *community.docker*(необходима для запуска docker-compose):

```
ansible-galaxy collection install community.docker
```

2. Установите обязательные переменные *tick_host* и *tick_user* соотвественно в ip-адрес(имя машины) и имя пользователя, имеющего права root на данных машинах.
Переменные устанавливаются в файле *[all.yml](inventory/group_vars/all.yml)*
