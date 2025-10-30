Данные заметки предназаначены для помощи в публикации материалов Obsidian через движок Hugo

# Как собрать сайт
1. Собирается с помощью ключей `--contentDir`, `--cleanDestinationDir` и `--destination ../docs`

hugo server --contentDir  ~/YandexDisk/Sync.\ Projects/Obsidian.Notes/Я.Практикум/ --cleanDestinationDir --destination ../docs 

# Настройка Obsidian
1. Убрать WikiLinks (при этом можно будет пользоваться [[, которые будут трансформироваться в Markdown Link) `Settigs -> File and Links -> Wikilings = OFF`
2. Установить плагин Wikilinks to MDLinks (P1)
3. Установить плагин TextFormat (P2)
4. Установить плагин Regexp Find/Replase (P3)


# Просмотр сайта
Локальный просмотр сайта при запущенном hugo `hugo server` [открыть](http://localhost:1313)

# Работа с сылками на другие страницы
1. Набрать [[ - для поиска нужно страницы
2. Внести страницу, сформируется обычная ссылка
3. Добавить отображаемое название ссылки ( ref "TITLE" )

Пример
`[Общий обзор языка Kotlin](Технологии.%20Язык%20Kotlin.md )`

[Hugo Docs](https://gohugo.io/render-hooks/images/)

# Работа с картинками
1. Hotkey для Wikilinks to MDLinks (P1) - Ctrl+Shift+L - конвертация ссылок из одного формата в другой
2. Стереть название файла из квадратных скобок. Можно использовать Regexp (P3)  `\!\[.*\]` заменить на `![]` 

1. Выбрать для TextFormat (Ctrl+P) - Text Format: Convert WikiLinks to plain MD links in selection
2. Убрать названия файлов
3. заменить png.md -> png
4. Удалить все пробелы в именах файлов - %20

Пример
`![](IMG_0574.png)`

# Работа с якорями

# Полезные ссылки
[Все настройки Hugo](https://gohugo.io/configuration/all/#ignorefiles)