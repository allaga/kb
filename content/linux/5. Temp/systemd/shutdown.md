$ shutdown -r +5
$ shutdown -r 15:00 'Message'
$ shutdown -r now
При завершении работы (в том числе и при перезагрузке) производится ряд очень важных действий, а именно синхронизация буферов ввода/вывода и размонтирование всех файловых систем. Именно поэтому очень важно правильно завершить работу системы.

$ shutdown +5
$ shutdown 15:00 'Message'
$ shutdown now

синтаксис команды
shutdown [OPTIONS...] [TIME] [WALL...]

сделать в виде таблицы, ты погодь у некоторых команд бывают не толко опции, но и параметры и т.д. надо учесть это

-P
-h - Завершение работы системы

-c Отменяет запланированное задание

-h The same as --poweroff, but does not override the action to take if it is "halt".
