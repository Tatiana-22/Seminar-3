# Инструкция по работе с Git

## Что таоке Git ?

***Git*** - самая популярная реализация распределённой системы контроля версий (версионность поддерживается и на сервере, и у каждого клиента). Самая распространнёной реализацией ***Git*** является (GitHub)[https://github.com]

## Подготовка репозитория
Для создание репозитория используется команда "git init". Для этого необходимо открыть в терминале папку с будущем репозиторием и написать "git init".

### Добавление файлов к коммиту
Для добовления файла к новому коммиту используется команда "git add". Используется она следущим образом: в терминале с папкой-репозиторием пишем *git add <название файла>*.

### Создание коммита
Для создание новой фиксации (коммита) используется команда *git commit*. для этого в терминале с папкой-репозиторием пишем *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***

## Журнал изменений
Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*.

## Перемещение между коммитами
Для перемещения на другую фиксацию(коммит) используется команда*git checkout*. Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш(номер), после чего в терминале с папкой-репозиторием надо написать *git checkout <хеш-кoммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Удаление веток
С операцией удаления над ветками справляется уже привычная команда git branch с параметром: *git branch -d и имя ветки*.

Git не позволит удалить ветку, у которой есть несохраненные изменения. Так мы избегаем ситуации, когда часть написанного кода будет безвозвратно утеряна. Если же мы уверены, что изменения в этой версии не нужны и их можно смело удалять, то вместо флага -d используем -D.