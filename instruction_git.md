# **Инструкция для работы с git**

![Логотип](git.jpeg)

## Что такое git

git  - это одна из реализаций распределенных систем контроля версий

## Подготовка репозитория

Что бы создать (инициализировать) иной репозиторий в текущей папке, нужно ввести в терминале команду:

    git init

## Сохранение изменений

После каждого введения новой информации в файл, нужно сохранить изменения. Внесение изменений сохраняется командой shift+S и далее в терминаое нужно ввести команду:

    git add имя файла

## Создание коммитов

Коммиты сущетсвуют для того, что бы можно было легко отслеживать изменения в файле. Можно ставить коммит как для каждого изменения самостоятельно, так и сделать команду для автоматического изменения в файле. Для того, что бы ввести коммит к конкретному файлу, нужно ввести команду:

    git commit -m "комментарий"

Для автоматического введения коммита к уже введеным ранее файлам:

    git commit -a "комментарий"

## Проверка текущего состояния файлов

Для того, что бы отследить все ли файлы внесены корректно, закоммичены и сохранены, а так же проверить текущий статус, нужно ввести команду:

    git status

## Отслеживание изменений

Так же существует команда для контроля за всеми изменениями в истории файла, где можно просмотреть кто, что и когда вносил в коммиты. С помощью нее можно отфильтровать изменения в коммитах или искать конкретные. Команда для просмотра всей истории изменений:

    git log 

Команда для просмотра всей истории изменений только с просмотром самого коммита:

    git log --oneline --all

Для перемещение между коммитами и просмотрами всех изменений в обратной или текущей последовательности, после команды git log нужно выбрать конкретные коммит скопировать его имя и вставить в строку ввода команды, после него встать файл изменения ДО какого мы хотели просмотреть или же наоборот. Команда для ввода:

    git checkout (имя), (имя)

После внесений каких либо изменений, нужно обязательно возвращаться к команде:

    git checkout master

   ## Сравнение изменений

   Для того, что бы отслежить что же конкретно поменялось в самом файле, какие текстовые или графические изменения были внесены, используется команда по аналогии с git checkout, когда мы вводим имя определенного комита до или после изменения. Только в данном конкретном случае мы просматриваем не коммит, а конкретное изменение внутри файла. Что бы проверить изменения, нужно ввести:

    git diff (имя), (имя) 

## Ветвления

Ветки в git используются для возможности работы не в основной ветке проекта, что бы можно было продолжать работу не зависимо от ветки master. Вносить изменения и потом сливать их в основную ветвь уже конечный, уверенный вариант. 

## Просмотр существующих веток

Для просмотра списка всех существующих веток нужно ввести команду:

    git branch
    
### Создание новых веток

Для создания новых веток нужно ввести команду:

    git branch (имя)


## Слияние веток

Для того, чтобы влить другую ветку в текущую нужно:
 - переключтится на ту ветку **куда** вливаем
 - ввести команду слияния, указав ту ветку, **которую** вливаем.

 Команда для слияния

    git merge (имя ветки)

### Удаление веток

Что бы удалить ветку нужно ввести команду:

    git branch -d (имя)

### Создание нового удаленного репозитория


### Отправка изменений в удаленный репозиторий
