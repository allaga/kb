# chgrp
Change group ownership.


## Synopsis
```console
chgrp [OPTION]... GROUP FILE...
chgrp [OPTION]... ‐‐reference=RFILE FILE...
```
Change the group of each `FILE` to `GROUP`. With `--reference`, change the group of each `FILE` to that of `RFILE`.


## Examples
```bash
# Изменение группы владельца
chgrp root ./directory/file
chgrp www-data ./directory/
```
