# Выполнено ДЗ №3

 - [+] Основное ДЗ
 - [+] Задание со *

## В процессе сделано:
1. В файле deployment.yaml readiness проба заменена на httpGet
2. Создан манифест service.yaml
3. Установлен ingress
4. Создан манифест ingress.yaml
5. В манифесте ingress.yaml добавлено rewrite правило и путь для /homepage

## Как запустить проект:
 1. kubectl apply -f namespace.yaml
 2. kubectl apply -f deployment.yaml
 3. kubectl apply -f service.yaml
 4. kubectl apply -f ingress.yaml

## Как проверить работоспособность:
 1. Изнутри k8s - wget http://10.109.86.236:8000 (ip сервиса)
 2. Из браузера - http://homework.otus:32463/homepage (предварительно указав в hosts запись)

## PR checklist:
 - [ ] Выставлен label с темой домашнего задания
