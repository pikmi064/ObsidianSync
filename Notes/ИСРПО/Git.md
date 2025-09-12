## **Настройка**


```bash
git config --global user.name "Ваше Имя"
git config --global user.email "your.email@example.com"
git config --global color.ui auto
```
---

## **Основные понятия**

- **Коммит** - снимок состояния файлов
    
- **Ветка** - линия разработки
    
- **HEAD** - указатель на текущее положение
    
- **Staging Area** - область подготовленных файлов
    
- **Working Directory** - рабочая директория
    

---

## **Базовые команды**

### **Инициализация**

``` bash
git init
git clone <url>
```

### **Статус и история**

``` bash
git status
git log
git log --oneline --graph --all
git log --oneline --graph main..
```

### **Работа с изменениями**
``` bash
git add <file>
git add .
git commit -m "message"
git commit -am "message"
git rm <file>
git mv <old> <new>
```

### **Отмена действий**

``` bash
git restore <file>
git restore --staged <file>
git commit --amend
git revert <commit>
```

---

## **Ветки**

### **Основные операции**

```bash
git branch
git branch <name>
git checkout <name>
git switch <name>
git checkout -b <name>
git switch -c <name>
git merge <branch>
git branch -d <name>
```

### **Rebase**

```bash

git rebase <branch>
git rebase -i HEAD~3
git rebase --continue
git rebase --abort
```

---

## **Удалённые репозитории**

### **Подключение**


```bash
git remote add origin <url>
git remote -v
git fetch
git fetch --all
```

### **Синхронизация**


``` bash
git pull
git pull --rebase
git push
git push -u origin <branch>
```

### **Работа с ветками**

```bash
git checkout -b main origin/main
git branch -u origin/<branch>
git push -u origin <branch>
```

---

## **Конфликты и их решение**

1. Редактируем файлы с конфликтами
    
2. Убираем маркеры <<<< ==== >>>>
    
3. Выполняем:
    


``` bash
git add <file>
git commit          # для merge
git rebase --continue # для rebase
```

---

## **Полезные команды**

### **Просмотр изменений**

``` bash
git diff
git diff --staged
git diff HEAD~3..HEAD
```
