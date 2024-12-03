# Практическая работа № 2 `mysyslog`

Этот репозиторий содержит систему `mysyslog` для ведения журналов в различных форматах.

## Подмодули
- `libmysyslog`: Основная библиотека для логирования.
- `libmysyslog-text`: Плагин для логирования в текстовом формате.
- `libmysyslog-json`: Плагин для логирования в формате JSON.
- `mysyslog-client`: Тестовое клиентское приложение.
- `mysyslog-daemon`: Демон для ведения журнала.

## Сборка
- 'make all': собирает все цели.
- 'make clean': удаляет все временные файлы.
- 'make deb': собирает deb-пакет.

## 
- mysyslog client: Запуск клиента: ./mysyslog-client -m "test message" -l INFO -d text -f /var/log/mysyslog.log
- mysyslog daemon: Файл конфигурации '/etc/mysyslog/mysyslog.cfg' и запуск демона: sudo systemctl start mysyslog-daemon
