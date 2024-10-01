## Лабораторная работа No1

**Задание :**

1\. Установите среду Linux :

Я устанавливаю `Ubuntu`, чтобы использовать операционную систему `Linux` .

![image](https://github.com/haha523/lab-1.linux/blob/fdcb31455a00e4e6a97fb9052e089b2bb2f124b4/app%20Ubuntu.png)

2\. Запустить терминал :

Сначала откройте терминал в `Ubuntu`. Вы можете выполнить поиск по запросу «Терминал» или использовать комбинацию клавиш `Ctrl + Alt + T`.

3\. Создание файла *script.bash* :

Откройте терминал и выполните команду для создания нового файла *script.bash*:

```bash
touch script.bash
```
Результат :
 
 `root@LAPTOP-AJ4C61LN:~# touch script.bash`

4\. Открытие и редактирование файла :

В терминале выполните команду для открытия файла в текстовом редакторе:  `gedit script.bash`

```bash
gedit script.bash
```
Результат :

`root@LAPTOP-AJ4C61LN:~# gedit script.bash`

5\. Пишите код для script :

В файле *script.bash*, введите следующий код :

```bash
#!/bin/bash

echo "Welcome to ITMO University"
```

Это простой script, который при запуске печатает `"Welcome to ITMO University"`.

![image](https://github.com/haha523/lab-1.linux/blob/780f6bef032d2aa0729235691c3419cfeb92247f/png%20for%20linux%201/png%20code%20linux%201.png)
6\. Запустите script :

Вернитесь в Terminal и введите следующую команду, чтобы запустить script :  `root@LAPTOP-AJ4C61LN:~# bash script.bash`

```bash
bash script.bash
```

![image](https://github.com/haha523/lab-1.linux/blob/33608dcd081c3cf4540988429c780e14442bef42/png%20for%20linux%201/png%20input%20linux%201.png).

Результат :

`root@LAPTOP-AJ4C61LN:~# bash script.bash`

`Welcome to ITMO University`

`root@LAPTOP-AJ4C61LN:~#`

7\. Модификация script :

Изменение скрипта для вывода имени:

```bash
#!/bin/bash

if [ "$#" -eq 0 ]; then
    echo "Usage: bash script.bash [Your Name]"
    exit 1
fi

NAME="$@"

echo "Welcome, $NAME"
```

![image](https://github.com/haha523/lab-1.linux/blob/a91cf3aeeba355060bbaec4fa21a5380c5dd357d/code%20linux%201.2.png)


8\. Сохраните и запустите script еще раз :

Сохраните файл *script.bash* и запустите script с таким именем:

```bash
bash script.bash Vasya Pupkin
```

`root@LAPTOP-AJ4C61LN:~# bash script.bash Vasya Pupkin`

`Welcome, Vasya Pupkin`

Результат :

`root@LAPTOP-AJ4C61LN:~# touch script.bash`

`root@LAPTOP-AJ4C61LN:~# nano script.bash`

`root@LAPTOP-AJ4C61LN:~# bash script.bash Vasya Pupkin`

`Welcome, Vasya Pupkin`

`root@LAPTOP-AJ4C61LN:~#`


![image](https://github.com/haha523/lab-1.linux/blob/13dcdb7ba59d86f17334aa679b8059ecf912872e/input%201.2.png)

 
Вы можете попробовать любое имя, и скрипт будет работать как положено.
