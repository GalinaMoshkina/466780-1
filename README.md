## Лабораторная работа 1

CTRL + ALT + T - открытие терминала

1. Создайем новый файл с именем `script.bash`

```bash
touch script.bash
```

![image](https://github.com/user-attachments/assets/1117571a-f63e-4b33-9a0c-ad93a4e10d5a)


2. С помощью текстового редактора `gedit` открываем созданный файл `script.bash` для редактирования. Для этого пишем в терминале

```bash
gedit script.bash
```
Изначально терминал не распознает `gedit` , поэтому его нужно установить:

![image](https://github.com/user-attachments/assets/1497367e-391d-4a59-9b47-bc4560a318ae)

![Снимок экрана (1287)](https://github.com/user-attachments/assets/4bc7df29-6c3f-464a-8bb0-eccd87f5fe77)


3. Вписываем следующий скрипт и сохраняем файл и закрываем текстовый редактор `gedit`

```bash
#!/bin/bash

echo "Welcome to ITMO University"
```

![Снимок экрана (1298)](https://github.com/user-attachments/assets/bd263d21-a30d-4e04-b73f-b93f692ac3a3)


4. Запускаем bash-скрипт, написав в терминале

```bash
bash script.bash
```
И выводится `Welcome to ITMO University`

![image](https://github.com/user-attachments/assets/b1bd8485-1fa3-495d-9ad8-640a0999ea5b)

### Задача

Модифицируем файл `script.bash` так, чтобы при его запуске в терминале в виде

```bash
bash script.bash Vasya Pupkin
```

Вывод был (для любых имен)

`Welcome, Vasya Pupkin`

1. Открываем файл `script.bash` с помощью `gedit`

```bash
gedit script.bash
```

2. Вписываем следующий скрипт, где `$*` - переменная в bash, которая представляет все аргуементы, переданные скрипту. Сохраняем файл и закрываем текстовый редактор `gedit`

```bash
#!/bin/bash

echo "Welcome, $*"
```

![Снимок экрана (1294)](https://github.com/user-attachments/assets/3a08bf23-9cc9-4f5d-a0fe-72ea9387f847)

3. Теперь запускаем bash-скрипт

![image](https://github.com/user-attachments/assets/540d6dcc-d902-4c99-864a-408022f21a61)
