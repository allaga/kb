# diff
#### `GNU Diffutils`
Compare files line by line.


## Synopsis
```console
diff [OPTION]... FILES
```
Coming soon...


## Options
| Option                    | Description                                  |
|---------------------------|----------------------------------------------|
| -r, --recursive           | Recursively compare any subdirectories found |
| -b, --ignore-space-change | Ignore changes in the amount of white space  |
| -w, --ignore-all-space    | Ignore all white space                       |
| -B, --ignore-blank-lines  | Ignore changes where lines are all blank     |


## Examples
```bash
# Рекурсивное сравнение файлов
diff -r ./directory/ ../directory/
```


## Notes
Строка из первого файла помечается символом `<`, а из второго файла - символом `>`.
