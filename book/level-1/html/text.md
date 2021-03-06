# Html и текст
В стародавние времена когда еще не было google, wikipedia, социальных сетей
а о сервисах вроде gmail или youtube и не могли мечтать и зародился html.

Основная цель - создать набор связанных между собой документов, естественно текстовых с
редкими вставками изображений отображение которых я выключал чтобы не съедали трафик
который я покупал по карточкам для своего dial-up модема

Хорошими примерами сайтов того времени можно считать например стандарты 
[RFC](https://tools.ietf.org/html/rfc791)
или [словарь эльфийских языков](http://tolkien.olmer.ru/arhiv/Slovar_pr1.htm)  для толкиенистов

В наше время очень часто забывают о том что основная цель сайта - донести информацию в наиболее
удобном и читаемом формате. 

Прежде всего сайт это документ, и как у любого формата 
документов в html должны присутствовать средства для создания обычных документов.
 
В наше время есть и более удобные форматы например markdown (на нем кстати и создана эта книга) 
или ReStructuredText
а так-же специфические не совсем удобные но мощные форматы вроде TeX. Но и в html можно создавать
прекрасные интерактивные документы.

В Microsoft Word и Libre Office есть средства экспорта в html. Так что для создания 
простого сайта можно и не изучать html - создать текст в Word и экспортировать его и ваш самый первый сайт готов.

Однако для нормального WEB разработчика знание html это как знание азбуки, так что начинаем погружение!

## Блочные и строчные теги

Документ может состоять из блоков текста / изображений / видео и тд.
И из строк которые могут быть расположены в этих блоках.

Блоки можно по разному располагать на экране, менять из размер и форму и по умолчанию занимает все свободное пространство.
Строчные элементы расположены внутри блоков и вписываются в размеры родительских блоков.

Самый первый наш блочный элемент это само тело сайта `body` а строчным элементом
являются любой текст в нем.

## шапка, статья, подвал, параграф и блок

На странице содержимое может быть расположено в блоках и первый тег для блоков
это `<div></div>` - этот тег не несет никакой смысловой нагрузки и его можно распологать на сайте
как вам угодно.

Любой текст состоит из абзацев и параграфов которые позволяют разбить сплошную портянку
текста на удобно читаемые и усваиваемые куски информации. В html для этих целей
используется тег `<p></p>`. 

Параграф в отличии от блока имеет отступы снизу и сверху, размер отступов по умолчанию определяется браузером.

В html5 введены теги:

- статья - `<article></article>`
- шапка - `<header></header>`
- подвал - `<footer></footer>`

Разницы между ними и `<div>` нет, кроме синтаксической. Если вы делаете ленту новостей, то для
списка анонсов лучше использовать `<div>` а для самой статьи - `<article>`

Если пользоваться терминами книги - то `<div>` - любой блок в книге, `<header>` - обложка
а `<footer>` - станица с информацией о книге в конце или на обратной стороне книги.

Поисковые системы лучше распознают структуру сайта если использовать `<header>`, `<article>` и `<footer>`

## Корешок книги

Как у книги есть корешок - так и у сайта есть тег `<aside>`
По сути он является аналогом `<div>` и несет только смысловую нагрузку которая указывает что он 
должен являться панелью сайта.
 
 







