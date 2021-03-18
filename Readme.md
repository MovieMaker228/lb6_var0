# Task 

[ссылка на методичку по лабораторке](https://knureigs.github.io/itech/lb/ITech2_MongoDB/index.html)

Вариант 0. Создать и заполнить БД для хранения информации о литературных ресурсах библиотеки (книгах, газетах, журналах и т.д.). Для описания множества литературных ресурсов достаточно использовать одну коллекцию. Каждый ресурс, представленный в виде документа в составе коллекции, характеризуется набором свойств (и каждый, возможно, своим собственным, особым набором). Например, книги могут характеризоваться названием, уникальным номером (ISBN), издательством, годом издания, количеством страниц, автором (авторов может быть больше одного). У каких-то книг какого-то из перечисленных для примера свойств может и не быть, или быть какое-то новое свойство (например, наличие в комплекте диска). Журналы характеризуются обычно названием, годом выпуска, номером. Помните, что нет жесткого ограничения на одинаковый набор полей для разных ресурсов, пользуйтесь преимуществами MongoDB. Запросы на выборку предполагают, что требуемые поля будут у какой-то части документов в коллекции - но совсем не обязательно, что у всех.

Предоставить пользователю возможность получения информации о:

1. литературе указанного издательства;

2. литературе, опубликованной за указанный временной период (учитывать год издания);

3. литературе указанного автора.

# Как развернуть это веб-приложение на локальном хосте?

## Работа с СУБД mongo через командную утилиту mongosh

Нужно чтобы был установлен сервер MongoDB. Нужно создать и заполнить БД данными при помощи mongosh (mongo shell).

Для того, чтобы заполнить БД надо выполнить в консоли mongo (mongosh) две команды: use и insertMany

Обе команды надо взять из файла dump.json

Результат успешного выполнения команды use:

![](screenshots/use.png)

В результате выполнения команды insert в коллекции должно быть 7 документов.

Результат успешного выполнения команды use:

![](screenshots/insert.png)

## Проверка наличия расширения php mongodb 

В phpinfo должен быть раздел mongodb:

![](screenshots/mongo-extension.png)

Если его нет, то надо устанавливать

## Установка PHP-библиотеки MongoDB

Необходимо добится появления папки vendor в папке проекта

Как это сделать - смотреть презентацию [здесь](https://www.dropbox.com/s/a57henlgz2dr59i/MongoDB_PHP.pdf?raw=1)







