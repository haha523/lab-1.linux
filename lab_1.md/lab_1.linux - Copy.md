## Лабораторная работа No1

**Задание 1:**

1\. Установите среду Linux :

Я устанавливаю `Ubuntu`, чтобы использовать операционную систему `Linux` .
![image](https://github.com/haha523/lab-1.linux/blob/fdcb31455a00e4e6a97fb9052e089b2bb2f124b4/app%20Ubuntu.png)
2\. Запустить терминал :

Сначала откройте терминал в `Ubuntu`. Вы можете выполнить поиск по запросу «Терминал» или использовать комбинацию клавиш `Ctrl + Alt + T`.

3\. Создание файла script.bash :

Откройте терминал и выполните команду для создания нового файла script.bash:

root@LAPTOP-AJ4C61LN:~# touch script.bash

4\. Открытие и редактирование файла :

В терминале выполните команду для открытия файла в текстовом редакторе:                 nano script.bash

root@LAPTOP-AJ4C61LN:~# nano script.bash

5\. Пишите код для script :

В файле script.bash, введите следующий код :

#!/bin/bash

echo "Welcome to ITMO University"

Это простой script, который при запуске печатает "Welcome to ITMO University".

6\. Запустите script :

Вернитесь в Terminal и введите следующую команду, чтобы запустить script :

root@LAPTOP-AJ4C61LN:~# bash script.bash

Результат :

root@LAPTOP-AJ4C61LN:~# bash script.bash

Welcome to ITMO University

root@LAPTOP-AJ4C61LN:~#

7\. Модификация script :

Изменение скрипта для вывода имени:

#!/bin/bash

if [ "$#" -eq 0 ]; then

`   `echo "Usage: bash script.bash [Your Name]"

else

`    `echo "Welcome, $\*"

fi

8\. Сохраните и запустите script еще раз :

Сохраните файл script.bash и запустите script с таким именем:

root@LAPTOP-AJ4C61LN:~# bash script.bash Vasya Pupkin

Welcome, Vasya Pupkin

Результат :

root@LAPTOP-AJ4C61LN:~# touch script.bash

root@LAPTOP-AJ4C61LN:~# nano script.bash

root@LAPTOP-AJ4C61LN:~# bash script.bash Vasya Pupkin

Welcome, Vasya Pupkin

root@LAPTOP-AJ4C61LN:~#

Вы можете попробовать любое имя, и скрипт будет работать как положено.
