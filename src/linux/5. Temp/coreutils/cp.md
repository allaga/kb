# cp
Copy files and directories.


## Synopsis
```console
cp [OPTION]... [‐T] SOURCE DEST
cp [OPTION]... SOURCE... DIRECTORY
cp [OPTION]... ‐t DIRECTORY SOURCE...
```
Copy `SOURCE` to `DEST`, or multiple `SOURCE(s)` to `DIRECTORY`.


## Options
`-R, -r, --recursive` - copy directories recursively


## Examples
```bash
# Стандартное копирование. Если file существует, то происходит перезапись
cp ./file ./directory/file

# Рекурсивное копирование содержимого каталога
cp -r ./directory1/* ./directory2/

# Резервное копирование
cp ./file ./file.backup
```
