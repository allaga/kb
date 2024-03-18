# chattr
#### `e2fsprogs`
Change file attributes on a Linux file system.


## Synopsis
```console
chattr [ -RVf ] [ -v version ] [ -p project ] [ mode ] files...
```
Coming soon...


## Options
| Option | Description                                                     |
|--------|-----------------------------------------------------------------|
| -R     | Recursively change attributes of directories and their contents |


## Attributes
| Attribute     | Description                                                                                                                                                                                                                                                                                                                            |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| immutable (i) | A file with the `i` attribute cannot be modified: it cannot be deleted or renamed, no link can be created to this file, most of the file's metadata can not be modified, and the file can not be opened in write mode. Only the superuser or a process possessing the `CAP_LINUX_IMMUTABLE` capability can set or clear this attribute |


## Examples
```bash
# Защита от случайного удаления
сhattr +i ./directory/file

# Рекурсивное снятие защиты от случайного удаления
chattr -R -i ./directory/
```
