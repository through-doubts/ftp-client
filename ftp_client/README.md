Автор: Москвин Илья

Консольная реализация ftp-клиента. 
Параметры запуска: host [login] [-P password] [-p port] [-e encoding] [-d] [-a].
Для более подробной информации о том, как правильно ввводить аргументы в программу,
запустите справку командой: ./program.py -h.
После запуска работа с программой осуществляется через ввод в консоль комманд,
поддерживаемых программой.
Для запуска используйте: ./program.py

Пример запуска: ./program.py 127.0.0.1 Name -P -p 21 -e cp1251 -d -a

Собственно поддерживаемые команды и примеры использования:

ls [remote-directory] - вывести список файлов содержащихся в remote-directory,
если директория не задана или не существует, то будет использована текущая директория

get remote-file [local-file] - скачать remote-file с сервера в local-file,
если local-file не указан, то загрузка произойдет в файл с таким же именем
как у файла на сервере. Команда также работает и для директорий, при скачивании
которых также скачивается и все дерево поддиректорий

help [command] - вывести справку по команде, если команда не указана,
то выведется список команд, поддерживаемых программой

send local-file [remote-file] - отправить local-file на сервер в файл с именем
remote-file, если remote-file не указан, то будет использовано имя local-file.
Команда также работает и для директорий, при загрузке на севрер которых также
загружается и все дерево поддиректорий

cd [remote-directory] - перейти в директорию remote-directory

reconnect - переподключиться к серверу

close - используется для закрытия соединения с сервером

exit - выход


