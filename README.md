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
   `git push origin main`

 [Ссылка на коммит для задания 1](https://github.com/nikdev96/my-homework/commit/e05d2127c448e592e01fb7e8c9ad73ec161daa0f)

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

[Ссылка на коммит для задания 2](https://github.com/nikdev96/my-homework/blob/main/.gitignore)


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


![Скрин шот из Network graph](https://github.com/nikdev96/8-03-hw/blob/main/network.png)


### Задание 4


1. Создаем новой ветки conflict и переключение на нее
`git checkout -b conflict`

2. Изменение файла test.sh и создание коммита в ветке conflict
`echo "Conflict change from conflict branch" >> test.sh`
`git add test.sh`
`git commit -m "Change in test.sh from conflict branch"`

3. Отправка изменений в ветке conflict на GitHub
`git push origin conflict`

4. Переключение на основную ветку main
`git checkout main`

5. Изменение файла test.sh в основной ветке и создание коммита
`echo "Different change in test.sh from main branch" >> test.sh`
`git add test.sh`
`git commit -m "Change in test.sh from main branch"`

6. Отправка изменений основной ветки на GitHub
`git push origin main`

7. Попытка слияния ветки conflict с основной веткой main
`git merge conflict`

8. Разрешение конфликта (выбор изменений из ветки conflict)
`Открыть test.sh, отредактировать, сохранить`

9. Добавление разрешенного конфликта в индекс и завершение коммита
`git add test.sh`
`git commit -m "Resolve conflict by taking changes from conflict branch"`

10. Пуш изменений основной ветки на GitHub
`git push origin main`

[Ссылка на граф коммитов](https://github.com/nikdev96/my-homework/network)