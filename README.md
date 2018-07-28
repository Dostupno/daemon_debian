# daemon_debian
# Демонизация процесса

# Установка
Скопируйте в /etc/init.d:

# Заменить <NAME> на название сервиса
cp "service.sh" "/etc/init.d/Название сервиса"
chmod +x /etc/init.d/Название сервиса

# Редактировать в файле
<NAME> = Название сервиса
<DESCRIPTION> = Описание сервиса
<COMMAND> = Исполняемый файл (для примера /home/myuser/.dropbox-dist/dropboxd)
<USER> = Пользователь

# Cтандартное использование
service Название сервиса start
service Название сервиса stop

# Добавить в автозагрузку:
update-rc.d Название сервиса  defaults
