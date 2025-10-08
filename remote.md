# Команды Git для работы с удаленным репозиторием

## Основные команды для записи в удаленный репозиторий

### Добавление изменений в индекс
```bash
git add .
# или для конкретного файла
git add filename.ext
```

### Создание коммита
```bash
git commit -m "Описание изменений"
```

### Отправка изменений в удаленный репозиторий
```bash
git push origin branch-name
# или для текущей ветки
git push
```

### Комбинированная команда (добавить, закоммитить и запушить)
```bash
git add . && git commit -m "Описание изменений" && git push
```

## Дополнительные полезные команды

### Проверка статуса репозитория
```bash
git status
```

### Просмотр истории коммитов
```bash
git log --oneline
```

### Проверка удаленных репозиториев
```bash
git remote -v
```

### Синхронизация с удаленным репозиторием
```bash
git pull origin branch-name
```

### Создание и переключение на новую ветку
```bash
git checkout -b new-branch-name
```

### Слияние веток
```bash
git merge branch-name
```

## Примеры использования

### Пример 1: Обычный workflow
```bash
git add .
git commit -m "Добавлен новый функционал"
git push origin main
```

### Пример 2: Работа с новой веткой
```bash
git checkout -b feature/new-feature
git add .
git commit -m "Реализован новый функционал"
git push origin feature/new-feature
```

### Пример 3: Быстрый коммит и пуш
```bash
git add . && git commit -m "Исправлены ошибки" && git push
```