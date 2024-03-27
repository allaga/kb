# column
Columnate lists.


## Synopsis
```console
column [options] [file ...]
```
The column utility formats its input into multiple columns. The util support three modes:

       columns are filled before rows
           This is the default mode (required by backward compatibility).

       rows are filled before columns
           This mode is enabled by option -x, --fillrows

       table
           Determine the number of columns the input contains and create a table. This mode is enabled by option -t, --table and
           columns formatting is possible to modify by --table-* options. Use this mode if not sure. The output is aligned to the
           terminal width in interactive mode and the 80 columns in non-interactive mode (see --output-width for more details).

       Input is taken from file, or otherwise from standard input. Empty lines are ignored and all invalid multibyte sequences are
       encoded by x<hex> convention.


## Options
`-s, --separator separators` - specify the possible input item delimiters (default is whitespace).

`-t, --table` - determine the number of columns the input contains and create a table. Columns are delimited with whitespace, by default, or with the characters supplied using the `--output-separator` option. Table output is useful for pretty-printing.

## Examples
```bash
# jkenfjkwe
column -s: -t /etc/passwd
```
