# find
#### `GNU Findutils`
Search for files in a directory hierarchy.


## Synopsis
```console
find [-H] [-L] [-P] [-D DEBUGOPTIONS] [-OLEVEL] [FILE...] [EXPRESSION]
```
Coming soon...


## Expressions
| Option | Description                                                   |
|--------|---------------------------------------------------------------|
| -R     | Recursively list attributes of directories and their contents |


## Examples
```bash
найти все симолические ссылки
find /bin/ -type l

Найти все файлы с именем file.txt
find / -name file.txt

найти файлы по маске
find / -name *.py

Найти пустые файлы
find . -empty

найти файлы, размер которых от 1 гбайт и больше
find ~ -size +1G
```
