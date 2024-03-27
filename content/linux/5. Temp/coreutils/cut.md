# cut
Remove sections from each line of files.


## Synopsis
```console
cut OPTION... [FILE]...
```
Print selected parts of lines from each `FILE` to standard output.

With no `FILE`, or when `FILE` is `-`, read standard input.


## Options
`-d, --delimiter=DELIM` - use `DELIM` instead of `TAB` for field delimiter

`-f, --fields=LIST` - select only these fields; also print any line that contains no delimiter character, unless the `-s` option is specified


## Examples
```bash
# fefwe
cut -f2 ./file

# Если нужно вывести первую и третью колонки айла
cut -f1,3 ./file

# Можно также указать диапазон выводимых колонок
cut -f1-3 ./file

# С помощью параметра -d можно указать другой разделитель
cut -f1 -d\| ./file
```


## Notes
По умолчанию в качестве разделителя колонок используется символ табуляции.
