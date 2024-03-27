# chmod
Change file mode bits.


## Synopsis
```console
chmod [OPTION]... MODE[,MODE]... FILE...
chmod [OPTION]... OCTAL‐MODE FILE...
chmod [OPTION]... ‐‐reference=RFILE FILE...
```


## Options



## Attributes



## Examples
```bash
chmod a+x <file>
chmod a-x <file>
chmod +x filr
chmod -x file
+s
chmod u=rwx,o=-r <file>
chmod 744 <file>
```

## Notes
Символьная нотация
Числовая нотация

7 – разрешены чтение, запись, исполнение
6 – разрешены чтение и запись
5 – разрешены чтение и исполнение
4 – разрешено только чтение
0 – ничего не разрешено

000 - 0
001 - 1
010 - 2
011 - 3
100 - 4
101 - 5
110 - 6
111 - 7

Для каталога право на выполнение означает право на просмотр содержимого каталога.

u - владелец файла;
g - группа владельца файла;
o - все остальные пользователи и группы;
a - все