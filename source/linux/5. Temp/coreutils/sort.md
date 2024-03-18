sort [OPTION]... [FILE]...
sort [OPTION]... ‐‐files0‐from=F

-r, --reverse - reverse the result of comparisons

-n, --numeric-sort - compare according to string numerical value

Вывод содержимого второй колонки, отсортированная в числовом пордке
cut -f2 <file> | sort -n

Вывод Список пользователей отсортив  в алфавитном порядке
cut -f1 -d: /etc/passwd | sort