# Команды git 
(инициализация / клонирование репозитория, создание коммита, отправка изменений на удаленный репозиторий / получение изменений с удаленного репозитория)

### 1. первоначальная настройка git 
(выполняется перед первым использованием git / для смены имени или email)
## git config --global user.name "your_name"  
## git config --global user.email your_email  

### 2. инициализация git репозитория
(необходимо перейти в папку с проектом, который будет инициализирован как git репозиторий)
## git init

### 3. индексация изменений
(проиндексированные файлы попадут в коммит)
## git add имя_файла 
например, git add index.html

### 4. коммит (фиксация) изменений
## git commit -m "commit message"

### 5. добавить в коммит все изменения
(команду git add в данном случае можно не выполнять)
## git commit -a "commit message"

### 6. добавление нового удаленного репозитория
## git remote add origin ссылка_на_репозиторий
например, git remote add origin https://github.com/ifmo-web-developer/html.git

### 7. отправить изменения на удаленный репозиторий
## git push -u origin master

### 8. склонировать существующий git репозиторий
## git clone ссылка на репозиторий
например, https://github.com/ifmo-web-developer/html.git

### 8. получить изменения из удаленного репозитория
## git pull

## Есть 2 варианта работы с удаленными репозиториями:
### 1. Клонирование существующего репозитория.
В данном случае необходимо один раз склонировать репозиторий командой git clone,
дальнейшие изменения получать командой git pull. Если вам необходимо отправить изменения в склонированный репозиторий, то индексируете их командой git add имя_файла, делаете коммит git commit -m "commit message" и отправляете командой git push 
### 2. Инициализация git репозитория на локальном компьютере и последующая отправка на удаленный репозиторий.
В таком случае выполняете один раз команду git init, индексируете изменения командой git add имя_файла, делаете коммит git commit -m "commit message", один раз добавляете новый удаленный репозиторий - git remote add origin ссылка_на_репозиторий, отправляете изменения - git push -u origin master. 
При последующих отправках изменений на удаленный репозиторий достаточно выполнить команды git add имя_файла, git commit -m "commit message" и git push

## Ссылки на ресурсы по системе контроля версий git:
### https://git-scm.com/book/ru/v1
### https://githowto.com/ru
