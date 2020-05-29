# Задание на дипломный проект «Облачный архиватор» первого блока «Основы языка программирования Python».

Облачные хранилища стали для человека уже нормой. Загрузить в облако альбом с фотографиями или поделиться какими-либо документами не составляет большой сложности. Но есть одна проблема — там может закончиться место. Было бы неплохо уметь архивировать самый большой и тяжёлый файл или папку и загружать обратно в облако. Так можно сохранить больше свободного места.

## Задание:
Нужно написать программу, которая будет:
1. Получать информацию по всем папкам в Я.Диске.
2. Искать среди них самый тяжёлый.
3. Скачивать файл на компьютер, где запущена программа.
4. Архивировать файл.
5. Загружать его обратно в ту же папку, откуда он был скачен.
6. Записывать информацию по измененному файлу в json-файл.

###Входные данные:
Пользователь вводит токен с [Полигона Яндекс.Диска](https://yandex.ru/dev/disk/poligon/)

###Выходные данные:
1. json-файл с информацией по файлу:
```javascript
    {
    “file_name”: “diplom.docx”,
    “size”: “идентификатор группы”,
    “path”: “disk:/Netology/diplom.docx”
    }
```
2. Измененный Я.диск, куда добавился новый архив.
​
​
### Обязательные требования к программе:
1. Использовать REST API Я.Диска и ключ, полученный с полигона.
2. Для архивации файлов или папки использовать библиотеку zipfile.
3. Опционально предлагать пользователю удалить с Диска файл/папку вместо загружаемого файла.
4. Сделать прогресс-бар для отслеживания процесса программы.
5. Код программы должен удовлетворять PEP8.
​
### Дополнительные требования к программе:
1. Выдача топ-10 файлов по размеру.
2. Запись в гугл-таблицу список файлов в табличном виде - название, каталог хранения, размер.
