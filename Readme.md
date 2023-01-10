# Инструкция по работе с Git

## Что таоке Git ?

## Подготовка репозитория

## Создание "сохранений"

## Перемещение между "сохранениями"
Для перемещения на другую фиксацию(коммит) используется команда*git checkout*. Для этого необходимо, как показано в прошлом пункте, в журнале изменений найти необходимый коммит и его хеш(номер), после чего в терминале с папкой-репозиторием надо написать *git checkout <хеш-кoммита>*. После выполнения этой команды мы попадаем в состояние **detached head**, в котором никакие следующие коммиты сохраняться не будут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Журнал изменений 

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Удаление веток