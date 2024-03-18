# chown
Change file owner and group.


## Synopsis
```console
chown [OPTION]... [OWNER][:[GROUP]] FILE...
chown [OPTION]... ‐‐reference=RFILE FILE...
```
chown changes the user and/or group ownership of each given file. If only an owner (a user name or numeric user ID) is given, that user is made the owner of each given file, and the files’ group is not changed. If the owner is followed by a colon and a group name (or numeric group ID), with no spaces between them, the group ownership of the files is changed as well. If a colon but no group name follows the user name, that user is made the owner of the files and the group of the files is changed to that user’s login group. If the colon and group are given, but the owner is omitted, only the group of the files is changed; in this case, chown performs the same function as chgrp. If only a colon is given, or if the entire operand is empty, neither the owner nor the group is changed.

Change the owner and/or group of each `FILE` to `OWNER` and/or `GROUP`. With `--reference`, change the owner and group of each `FILE` to those of `RFILE`.


## Options
`-R, --recursive` - operate on files and directories recursively


## Examples
```bash
# Изменение владельца и группы
chown root:root ./directory/

# Изменение владельца
chown www-data ./file
```
