
Поиск слова бубунту в файлах
grep "Ubuntu" file1.txt file2.txt file3.txt ...

Если файлов много и нужно произвести по всем, тогда лучше испльть команду 

grep "Ubuntu" file* 


examples

Отфильтровать информацию об устройствах компании Intel из сообщения ядра 

dmesg | grep "intel"

Поиск внутри файла

grep "Intel" <file>

Нужно получить строки, не содержащие упоминания про Intel

grep -v "Intel" <file>

SYNOPSIS
       grep [OPTION...] PATTERNS [FILE...]
       grep [OPTION...] -e PATTERNS ... [FILE...]
       grep [OPTION...] -f PATTERN_FILE ... [FILE...]

       -v, --invert-match
              Invert the sense of matching, to select non‐matching lines.