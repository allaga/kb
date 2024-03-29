# Linux


- https://github.com/hcodes/yaspeller
- https://marketplace.visualstudio.com/items?itemName=lextudio.restructuredtext


Эффективно сможет работать с Linux вообще и на сервере в частности только тот, кто освоил принципы работы в командной строке. Поэтому программы с GUI старайся в большей мере не использовать.

Почему важно писать короткую заметку? Ответ в том, что нам нужно быстро просматривать свой материал. Кроме того, встретившись с этой заметкой, память стриггерится и в голове всплывет контекст, вплоть до того, как эта заметка писалась. Однако, наш мозг - потемки. И на случай, если нужно погрузиться в подробности, мы и оставляем источник. Причем, максимально подробный путь.

А что же с практикой? В предисловии ко всем книгам по разработке написано, что практика - наше всё и необходимо воспроизвести все примеры. Нельзя не согласиться с авторами этой идеи. Однако, не нужно механически переписывать то, что предлагает читателю автор книги.

Так, пример из области объектно-ориентированного программирования с фигурой, от которой наследуются треугольник, прямоугольник и круг вряд ли западет в душу и принесет удовольствие. И самое неприятное - он вряд ли потом вспомнится. В идеале, придумать что-то своё. Вместо упомянутых выше безликих фигур придумайте классы/расы из какой-нибудь игры в жанре RPG (Computer Role-Playing Game): танки, самолеты, что угодно, что будет интересным и запоминающимся конкретно вам. 

Важно помнить, что чем больше прочитанного по схожей тематике, тем быстрее понимаешь концепции и мысли другого автора. Некоторые книги после достаточного опыта можно читать со скоростью художественной литературы. Количество прочитанного текста никак не влияет на дикцию и написание тех, у кого дислексия.

Кроме того, если нужно пройти собеседование или assessment, у вас есть отличный материал, доказывающий, что вы действительно читаете и прорабатываете материал, да еще и имеете базу знаний, которая поможет эффективно выполнять свою работу. Получается, есть не только слова, но и конкретная фактура.


# SysRq
У некоторых пользователей комбинации клавиш с `<SysRq>` просто не срабатывают. А все из-за того, что в ряде дистрибутивов по умолчанию они отключены.

```bash
# nano /etc/sysctl.conf
>>> kernel.sysrq=1
$ reboot
```

`<Alt> + <SysRq> + <B>` - эквивалентно перезагрузке компьютера кнопкой Reset
`<Alt> + <SysRq> + <E>` - послание всем процессам (кроме подсистемы инициализации) сигнала SIGTERM. После этого будут запущены только ядро и подсистема инициализации
`<Alt> + <SysRq> + <K>` - завершение всех процессов

`<Ctrl> + <Alt> + <F1-6>` `<Alt> + <F1-6>` - переключение между консолями и графическим режимом

`<Ctrl> + <Alt> + <Del>` - перезагрузка компьютера из консольного режима


Computer Science
Docs as Code
Dynamic Host Configuration Protocol
Everything as Code
Fast Ethernet
Gigabit Ethernet
Initial ramdisk
SIGTERM
SOHO (бизнес)
Small office/home office
Softlanding Linux System
Super (клавиша)
SysRq
Trivial File Transfer Protocol
UNIX
Universally unique identifier
Usenet
Windows (клавиша)
https://dns.yandex.ru/
https://fontawesome.com/
https://fonts.google.com/
https://ifconfig.co/
https://tinkercad.com/
https://writethedocs.org/
root
Аптайм
Витая пара
Выключение вычислительной системы
Гибернация (операционные системы)
Графический интерфейс пользователя
Ждущий режим
Звёздочка (типографика)
Кабель категории 5
Кабель категории 6
Компьютер
Косая черта
Лаборатории Белла
Линус Торвальдс
Неизменяемый объект
Неравенство
Обратная косая черта
Операционная система
Перезагрузка
Проблема курицы и яйца
Рабочий стол
Репозиторий
Сервер (аппаратное обеспечение)
Сервер (программное обеспечение)
Системный вызов
Среда рабочего стола
Тильда
Тонкий клиент
Фреймовый оконный менеджер
Эндрю Таненбаум
Ядро Linux
Ядро операционной системы


Livepatch
Ubuntu Pro
badblocks -v <device>
dmidecode
iwconfig
iwlist <interface> scan
less /proc/cpuinfo
less /proc/meminfo
less /proc/mounts
lshw
lsmod
lspci
lsusb
sudo hdparm -t /dev/sdc
sudo pro attach <token>


# Linux Distributions
- Clonezilla Live
- Fedora Server
- Ubuntu Server

# Command Line Interface
- GNU Screen
- GNU Wget
- Midnight Commander
- https://github.com/FFmpeg/FFmpeg
- https://github.com/certbot/certbot
- https://github.com/curl/curl
- https://github.com/htop-dev/htop
- https://github.com/rakshasa/rtorrent

# Graphical User Interface
- Chrome
- KeePassXC
- Visual Studio Code
