# Вывод содержимого каталога
$ ls <dir>
Показ индексных дескрипторов файлов
ls -i

ls -l

- символ файла

d - символ каталога

b - блочное устройсто

c - символьное устройство

p - FIFO-канал

s - сокет

l - символ ссылки

. - тукещий каталог
.. - родительский каталог
~ - домашний каталог пользователя

синтаксис

ls *.zip

ls [OPTION]... [FILE]...

-F, --classify[=WHEN]
              append indicator (one of */=>@|) to entries WHEN

-R, --recursive
              list subdirectories recursively


-r, --reverse
              reverse order while sorting


-a, --all
              do not ignore entries starting with .

-i, --inode
              print the index number of each file


-l     use a long listing format

-r, --reverse
              reverse order while sorting

-t     sort by time, newest first; see --time

-S     sort by file size, largest first

-h, --human-readable - with -l and -s, print sizes like 1K 234M 2G etc.