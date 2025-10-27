# 🚀 Основные команды Git Bash

Краткий справочник по наиболее часто используемым командам Git и Bash для повседневной разработки.

## 📁 Навигация в файловой системе

| Команда | Описание | Пример |
|---------|-----------|---------|
| `pwd` | Показать текущую директорию | `pwd` |
| `ls` | Список файлов и папок | `ls -la` |
| `cd` | Перейти в директорию | `cd projects` |
| `cd ..` | Перейти на уровень выше | `cd ..` |
| `cd ~` | Перейти в домашнюю директорию | `cd ~` |
| `mkdir` | Создать директорию | `mkdir new-project` |
| `rmdir` | Удалить пустую директорию | `rmdir old-folder` |

## 📊 Работа с файлами

| Команда | Описание | Пример |
|---------|-----------|---------|
| `touch` | Создать файл | `touch index.html` |
| `cat` | Показать содержимое файла | `cat README.md` |
| `cp` | Копировать файл | `cp file1.txt file2.txt` |
| `mv` | Переместить/переименовать файл | `mv old.txt new.txt` |
| `rm` | Удалить файл | `rm file.txt` |
| `nano` | Редактировать файл в nano | `nano config.txt` |

## 🔧 Основные команды Git

### Настройка Git
```bash
git config --global user.name "Ваше Имя"
git config --global user.email "your.email@example.com"
git config --list

git init                        # Инициализировать новый репозиторий
git clone <url>                 # Клонировать удаленный репозиторий

git status                      # Показать статус изменений
git add <file>                  # Добавить файл в индекс
git add .                       # Добавить все изменения в индекс
git commit -m "Сообщение"       # Закоммитить изменения
git commit -am "Сообщение"      # Добавить и закоммитить все изменения

git log                         # Полная история коммитов
git log --oneline               # Краткая история коммитов
git log --graph                 # История с визуализацией веток
git log --oneline --graph --all # Вся история с графиком
git show <commit>               # Показать изменения в коммите
git show HEAD                   # Показать последний коммит

git log --oneline              # Покажет хеши коммитов (первые 7 символов)
git show abc1234               # Показать коммит с хешем abc1234
git checkout abc1234           # Переключиться на коммит с хешем abc1234

# HEAD - указатель на текущий коммит
git show HEAD                  # Текущий коммит
git show HEAD~1                # Предыдущий коммит
git show HEAD~2                # Два коммита назад

git status                      # Показать статусы всех файлов
git status -s                   # Короткий формат статуса

git add file.txt               # Перевести из modified → staged
git restore --staged file.txt  # Перевести из staged → modified
git commit                     # Перевести из staged → committed

git restore file.txt           # Откатить изменения (modified → unmodified)
git rm file.txt                # Удалить файл и добавить удаление в staged

git commit -m "feat: добавить новую функциональность"
git commit -m "fix: исправить баг в расчетах"
git commit -m "docs: обновить документацию"
git commit -m "style: форматирование кода"
git commit -m "refactor: изменить структуру кода"
git commit -m "test: добавить тесты"

feat: добавить аутентификацию пользователя

- Реализовать логин/логаут через JWT
- Добавить валидацию форм
- Настроить защищенные маршруты

Closes #123

alias gs='git status'
alias ga='git add'
alias gc='git commit -m'
alias gp='git push'
alias gl='git log --oneline --graph'
alias gco='git checkout'
alias gd='git diff'

git log --grep="bug"           # Найти коммиты по сообщению
git log -S "functionName"      # Найти коммиты по изменению кода
git log --since="2024-01-01"   # Коммиты с определенной даты

git log --grep="bug"           # Найти коммиты по сообщению
git log -S "functionName"      # Найти коммиты по изменению кода
git log --since="2024-01-01"   # Коммиты с определенной даты

git diff                       # Непроиндексированные изменения
git diff --staged              # Проиндексированные изменения
git diff HEAD~1 HEAD           # Изменения между коммитами


## 📁 Как сохранить:

1. **Откройте Notepad**
2. **Скопируйте ВЕСЬ текст выше** 
3. **Вставьте в Notepad**
4. **Сохраните как** `README.md` (обязательно с расширением `.md`)
5. **В типе файла выберите "Все файлы"**, чтобы не получилось `README.md.txt`

## 📍 Куда сохранять:

Сохраните файл в вашу папку проекта:


## ✅ После сохранения в Git Bash:

```bash
# Перейдите в папку проекта
cd /e/AQA/git-mini-lesson

# Проверьте что файл есть
ls -la README.md

# Добавьте в Git
git add README.md
git commit -m "Добавить полную шпаргалку по Git"
git push





















