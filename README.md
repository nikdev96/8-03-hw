# Домашнее задание к занятию "Git 8-01.md" - `Селиверстов Никита`


### Задание 1



1. Зарегистрировал аккаунт на GitHub.
2. Создали новый публичный репозиторий на GitHub и инициализировали его с файлом README.md.
3. Склонировали репозиторий на локальный компьютер с помощью команды `git clone https://github.com/nikdev96/my-homework`
   `cd main`
4. Настроили Git, указав имя пользователя и email с помощью команд:
   `git config --global user.name "мое имя"`
   `git config --global user.email "мое мыло"`
5. Внесли изменения в файл README.md, добавив произвольный текст.
6. Проверили статус изменений с помощью команды `git status`, чтобы увидеть, что файл изменен.
   `git add README.md`
   `git commit -m "Initial commit"`


### Задание 2



1. Создал файл .gitignore в корневой директории репозитория
2. Добавил правила в .gitignore для игнорирования файлов с расширением .pyc и директории cache. Содержимое файла .gitignore:
   `*.pyc`
   `cache`
3. Добавил файл .gitignore в индекс.
4. Создал коммит с описанием и отправили изменения на GitHub.
Создаем файла .gitignore  
`touch .gitignore`  
Добавление правил в .gitignore  
Проверка статуса изменени  й
`git status`  
Добавление .gitignore в индекс  
`git add .gitignore`  
Создание коммита  
`git commit -m "Add .gitignore with rules to ignore .pyc files and cache directory"`  
Отправка коммита на GitHub  
`git push origin main`  


### Задание 3


1. Создал новую ветку dev и переключился на нее.
2. В ветке dev создал файл test.sh с произвольным содержимым.
3. Сделал несколько коммитов с изменениями в test.sh и отправили их на GitHub.
4. Переключился обратно на основную ветку main.
5. В основной ветке создал файл main.sh с произвольным содержимым, сделал коммит и отправили его на GitHub.
6. Сделал слияние ветки dev с основной веткой main.
7. Не удалял ветку dev после слияния.

```
# Создание новой ветки dev и переключение на нее
git checkout -b dev

# Создание файла test.sh с произвольным содержимым
echo "echo Hello from test.sh" > test.sh

# Добавление файла и создание первого коммита в ветке dev
git add test.sh
git commit -m "Add initial version of test.sh"

# Изменение файла и создание второго коммита
echo "echo Another line in test.sh" >> test.sh
git add test.sh
git commit -m "Update test.sh with additional line"

# Отправка изменений в ветке dev на GitHub
git push origin dev

# Переключение на основную ветку
git checkout main

# Создание файла main.sh и коммит в основной ветке
echo "echo Hello from main.sh" > main.sh
git add main.sh
git commit -m "Add main.sh file for team development"

# Отправка коммита основной ветки на GitHub
git push origin main

# Слияние ветки dev с основной веткой main
git merge dev

# Пуш после слияния
git push origin main

```


![Скрин шот из Network graph](https://printskrin.ru/i/snimok-e-krana-2024-11-12-v-204950.SUnJyP)


### Задание 4



1. `Заполните здесь этапы выполнения, если требуется ....`
2. `Заполните здесь этапы выполнения, если требуется ....`
3. `Заполните здесь этапы выполнения, если требуется ....`
4. `Заполните здесь этапы выполнения, если требуется ....`
5. `Заполните здесь этапы выполнения, если требуется ....`
6. 

```
Поле для вставки кода...
....
....
....
....
```

`При необходимости прикрепитe сюда скриншоты
![Название скриншота](ссылка на скриншот)`