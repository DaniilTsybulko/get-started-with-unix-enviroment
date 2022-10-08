# **Отчёт по лабораторной работе № 1-2** по курсу "Фундаментальная информатика"

<b>Студент группы:</b> М80-108Б-22 Цыбулько Даниил Викторович, № по списку: 24 

<b>Контакты e-mail:</b> <ins>daniil.tsybulko.mai@gmail.com</ins>

<b>Работа выполнена:</b> «8» октября 2022 г.

<b>Преподаватель:</b> асп. каф. 806 Сахарин Никита Александрович

<b>Входной контроль знаний с оценкой:</b> <ins>   </ins>

<b>Отчет сдан</b> _________, <b>итоговая оценка</b> ____

<b>Подпись преподавателя:</b> ________________

## 1. Тема 
Операционная среда UNIX 

## 2. Цель работы 
Изучение и освоение программного обеспечения ОС UNIX и приобретение навыков, необходимых для выполнения курсовых и лабораторных работ в среде UNIX.

## 3. Задание (вариант № —)
Изучение команд и утилит bash.

## 4. Оборудование
<b>Процессор: </b>AMD Ryzen 5 3500U with Radeon Vega Mobile Gfx 2.10 GHz<br/>
<b>ОП:</b> 8ГБ <br/>
<b>Монитор:</b> 1920*1080 <br/>
## 5. Програмное обеспечение
<b>Опереционная система семейства: VirtualBox 6.1.38 - Ubuntu 22.04.1 LTS  <br/>
<b>Интерпретатор команд:</b> bash, версия 5.1.16<br/>
<b>Система программирования:</b> --, версия --<br/>
<b>Редактор текстов:</b> emacs, версия **28.2**<br/>
<b>Утилиты операционной системы:</b> cd, pwd, ls, cp, mc, mkdir, rmdir, cat, man, ps,rm<br/>
<b>Прикладные системы и программы:</b> gnuplot<br/>
<b>Местанохождение и имена файлов программ и данных на домашнем компьютере:</b> home/daniil_ts<br/>
## 6. Идея, метод, алгоритм решения задачи (в формах: словесной, псевдокода, графической [блок-схема, диаграмма, рисунок, таблица] или формальные спецификации с пред- и постусловиями)
Изучить основы программного обеспечения ОС UNIX
Ввод команд:
1. ```ls -l/-A/-lAF``` – ознакомление с содержимым директории
2. ```whoami``` – определение имени пользователя
3. ```hostname``` – определение терминала, котором ведётся работа
4. ```date``` – определение даты
5. ```tty``` – определение номера группы имени пользователя
6. ```uname -a``` – определение сетевого имени машины
7. ```finger daniil_ts``` – отображение полного имени и другой информации о пользователе
8. ```pwd``` – отображение полного пути к текущей директории
9. ```sudo ruptime``` – узнать, какие узлы сети в настоящий момент доступны, а какие нет
10. ```sudo rwho``` – узнать, какие пользователи работают на всех доступных UNIX-машинах
11. ```uptime``` – показывает текущее время, время работы после загрузки, количество  текущих пользователей и  нагрузку за последние 1, 5, 15 минут
12. ```man``` – получение оперативной документации по командам UNIX
13. ```cd``` – переход в другую директорию
14. ```ps``` - процессор
15. ```emacs``` – текстовый редактор
16. ```cp``` – копировать
17. ```cat``` – создание нового файла с возможностью записи/копировать
18. ```touch``` – создание пустого файла, если его нет. Если файл есть, то команда установит дату обращения в текущий момент времени 
19. ```rm``` – удаление
20. ```mv``` – перемещение
21. ```mkdir``` – создание директории
22. ```rmdir``` – удаление директории
23. ```gnuplot``` – утилита графики для построения двух- и трехмерных графиков
24. ```chmod +x ./myscript``` – делает скрипт исполняемым
25. ```./myscript``` – запуск скрипта
26. ```exit``` – выход
27. ```vim``` – текстовый редактор
    
## 7. Сценарий выполнения работы
- Изучить литературу по OC UNIX
- Просмотреть демонстрационный материал в лабораторной аудитории
- Приобрести основные навыки работы в OC UNIX
- Освоить навигацию в иерархической файловой системе OC UNIX
- Научиться манипулировать с файлами 
- Ознакомиться с утилитой графики 
- Научиться писать и запускать скрипты
- Запротоколировать сеанс
Пункты 1-7 отчета составляются сторого до начала лабораторной работы.
Допущен к выполнению работы.  
<b>Подпись преподавателя</b> ________________    
## 8. Распечатка протокола
```
daniil_ts@daniil-VirtualBox:~$ dir
abc     f2.txt  gnuplot  s.sh       text.txt  Документы  Изображения  Общедоступные  Шаблоны
f1.txt  f3.txt  snap     text2.txt  Видео     Загрузки   Музыка       Рабочий\ стол
daniil_ts@daniil-VirtualBox:~$ who
daniil_ts tty2         2022-10-08 00:22 (tty2)
daniil_ts pts/0        2022-10-08 03:04 (10.0.2.2)
daniil_ts@daniil-VirtualBox:~$ pwd
/home/daniil_ts
daniil_ts@daniil-VirtualBox:~$ ps
    PID TTY          TIME CMD
   4401 pts/0    00:00:00 bash
   4438 pts/0    00:00:00 ps
daniil_ts@daniil-VirtualBox:~$ whoami
daniil_ts
daniil_ts@daniil-VirtualBox:~$ hostname
daniil-VirtualBox
daniil_ts@daniil-VirtualBox:~$ date
Сб 08 окт 2022 03:06:01 MSK
daniil_ts@daniil-VirtualBox:~$ touch f4.txt
daniil_ts@daniil-VirtualBox:~$ echo iamdaniil > f4.txt
daniil_ts@daniil-VirtualBox:~$ cat f4.txt
iamdaniil
daniil_ts@daniil-VirtualBox:~$ cp f5.txt f6.txt
cp: не удалось выполнить stat для 'f5.txt': Нет такого файла или каталога
daniil_ts@daniil-VirtualBox:~$ cp f4.txt f1.txt
daniil_ts@daniil-VirtualBox:~$ cat f4.txt f1.txt > f3.txt
daniil_ts@daniil-VirtualBox:~$ cat f3.txt
iamdaniil
iamdaniil
daniil_ts@daniil-VirtualBox:~$ rm f3.txt f1.txt
daniil_ts@daniil-VirtualBox:~$ mkdir lab course
daniil_ts@daniil-VirtualBox:~$ cp f4.txt ~/lab/
daniil_ts@daniil-VirtualBox:~$ cp f4.txt ~/course/
daniil_ts@daniil-VirtualBox:~$ rm f4.txt
daniil_ts@daniil-VirtualBox:~$ cd lab
daniil_ts@daniil-VirtualBox:~/lab$ ls
f4.txt
daniil_ts@daniil-VirtualBox:~/lab$ rm f4.txt
daniil_ts@daniil-VirtualBox:~/lab$ ls
daniil_ts@daniil-VirtualBox:~/lab$ ls -a
.  ..
daniil_ts@daniil-VirtualBox:~/lab$ rmdir ~/course/
rmdir: не удалось удалить '/home/daniil_ts/course/': Каталог не пуст
daniil_ts@daniil-VirtualBox:~/lab$ cd course
-bash: cd: course: Нет такого файла или каталога
daniil_ts@daniil-VirtualBox:~/lab$ cd
daniil_ts@daniil-VirtualBox:~$ cd course
daniil_ts@daniil-VirtualBox:~/course$ rm f4.txt
daniil_ts@daniil-VirtualBox:~/course$ cd
daniil_ts@daniil-VirtualBox:~$ rmdir ~/course/
daniil_ts@daniil-VirtualBox:~$ ls
 abc      gnuplot   snap   text2.txt   Видео       Загрузки      Музыка         'Рабочий стол'
 f2.txt   lab       s.sh   text.txt    Документы   Изображения   Общедоступные   Шаблоны
daniil_ts@daniil-VirtualBox:~$ touch x.txt
daniil_ts@daniil-VirtualBox:~$ ls
 abc      gnuplot   snap   text2.txt   x.txt   Документы   Изображения   Общедоступные   Шаблоны
 f2.txt   lab       s.sh   text.txt    Видео   Загрузки    Музыка       'Рабочий стол'
daniil_ts@daniil-VirtualBox:~$ mv x.txt ~/lab/
daniil_ts@daniil-VirtualBox:~$ cd lab
daniil_ts@daniil-VirtualBox:~/lab$ ls
x.txt
daniil_ts@daniil-VirtualBox:~$ gnuplot

        G N U P L O T
        Version 5.4 patchlevel 2    last modified 2021-06-01

        Copyright (C) 1986-1993, 1998, 2004, 2007-2021
        Thomas Williams, Colin Kelley and many others

        gnuplot home:     http://www.gnuplot.info
        faq, bugs, etc:   type "help FAQ"
        immediate help:   type "help"  (plot window: hit 'h')

Terminal type is now 'wxt'
gnuplot> plot sin(x)
```
![Снимок экрана 2022-10-08 034127](https://user-images.githubusercontent.com/113765458/194678879-9a4e52d2-6fb2-4e43-bfc5-87972277640e.png)
```
gnuplot> set xrange [0 to 1]
gnuplot> set yrange [0 to 1]
gnuplot> plot cos(x)
```
![Снимок экрана 2022-10-08 034917](https://user-images.githubusercontent.com/113765458/194679198-b4f19afe-6708-445c-856b-f075e461e2b3.png)

## 9. Дневник отладки должен содержать дату и время сеансов отладки и основные события (ошибки в сценарии и программе, нестандартные ситуации) и краткие комментарии к ним. В дневнике отладки приводятся сведения об использовании других ЭВМ, существенном участии преподавателя и других лиц в написании и отладке программы.

| № |  Лаб. или дом. | Дата | Время | Событие | Действие по исправлению | Примечание |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| 1 | дом. | 08.10.2022 | 3:50 | Выполнение лабораторной работы | - | - |    
## 10. Замечания автора по существу работы

## 11. Выводы
Было выяснено, что в OC UNIX есть множество полезных утилит, которые облегчают работу в этой системе. Были изучены некоторые из них. Освоены навигация в файловой системе, создание, удаление файлов и директорий. В результате выполнения работы, были приобретены навыки, которые будут полезны для выполнения других лабораторных работ.

Недочёты при выполнении задания могут быть устранены следующим образом: —

<b>Подпись студента:</b> ____________________
