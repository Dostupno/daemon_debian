# Демонизация процесса (daemon debian)

# Установка
```sh
cp "service.sh" "/etc/init.d/Название сервиса"
chmod +x /etc/init.d/Название сервиса
``` 
# Редактировать в файле
* `<NAME>` = Название сервиса
* `<DESCRIPTION>` = Описание сервиса
* `<COMMAND>` = Исполняемый файл (для примера /home/user/./binfile)
* `<USER>` = Пользователь

# Cтандартное использование
```sh
service Название сервиса start
service Название сервиса stop
```
# Добавить в автозагрузку:
```sh
update-rc.d Название сервиса  defaults
```
