# Инструкция по работе с Markdown

## Заголовки в языке Markdown
Для создания заголовка в языке Markdown используетя символ "#" в начале строки. Колличество символов "#" обозначает уровень заголовка. Заголовок первого уровня самый **Большой.**

## Курсивное и жирное выделение
Для использования *курсивного текста* необходимо этот текст обрамить в символы звездочка. для использования **жирного текста** необходимо обрамить этот текст символами 2-х звездочек. для использования ***жирного курсивного текста*** необходимо этот текст обрамить в символы 3-х звездочек. Для использования ~~зачеркнутого текста~~ необходимо текст обрамить символами ~~. Алтернативный синтаксис - использование знака "_" по тем же правилам.

## Списки в языке Markdown
Для организации маркерованного списка используются знаки *, + и -. От них зависит вид маркеров. Чтоб сделать многоуровневый список, нужно будет сделать отступы (4 или 8 пробелов).
* Текст 1
    - Текст 2
        + Текст 3
        
Для нумерованных списков используют цифры
1. Текст 1
2. Текст 2

## Горизонтальные разделители
Для разделения в Markdown текста горизонтальными разделителями служат три или более дефиса, звездочки или знака равно (-, *, =).

Текст 1
-------------
Текст 2
*********
Текст 3
====

## Параграфы, абзац
Для оформления абзацев в языке Markdown блок текста автоматически преобразуется в параграф. Для вставки пустой строки необходимо два раза поставить символ переноса строки (нажать на Enter).

Абзацы создаются при помощи пустой строки. Если вокруг текста сверху и снизу есть пустые строки, то текст превращается в абзац.

Чтобы сделать перенос строки вместо абзаца,  
нужно поставить два пробела в конце предыдущей строки.

## Код
Для оформления блока кода используется обратный апостроф ` вокруг кода. Три символа для многострочного кода и один для однострочного:
```
$a = 5;
$b = 7;
```

`echo $c;`

так же для выделения кода можно использовать четыре пробела или табуляцию:

    print array

## Цитаты
Для их оформления применяется знак ">". 

Пример:

> Выберите себе работу по душе, и вам не придется работать ни одного дня в своей жизни. Конфуций

## Ссылки
Существует два варианта оформления ссылок. 
Первый - обычная вставка в текст:

[Программа Visual Studio Cod] (https://code.visualstudio.com/ VSCod)

Второй вариант - оформление ссылки в виде сноски.

Для скачивания git воспользуйтесь [Windows] [1] [macOS] [2] [Linux] [3]

[1] https://git-scm.com/download/win "Windows"

[2] https://git-scm.com/download/mac "macOS"

[3] https://git-scm.com/download/linux "Linux"

## Изображения
Изображения помещаются на страницу также, как и ссылки, с одним отличием: в начале записи используется знак "!"

![Фото собаки](media-share.jpg)

## Таблицы
Для построения таблиц используются символы "-", "_", "|". Для выравнивания текста внутри ячеек используются знаки ":" в строке, отделяющей заголовок от основной таблицы.

  Имя   |  Возраст
--------|:---------:
Илья    | 33
Анна    | 27
Игорь   | 30

## Спецсимволы
Чтоб вставить в текст, например, знак больше ">", а не выделить текст в виде цитаты, необходимо поставить перед ним обратный слеш (\) вот так: \* или \>

## Кодовые фрагменты строк
Чтобы отметить фрагмент строки, содержащий код, необходимо окружить его обратными апострофами «`». При использовании кодовых фрагментов строк текст будет отображаться в виде моноширинного шрифта. В отличие от блоков кода, кодовый фрагмент позволяет поместить код внутрь обычного абзаца текста. Кодовый фрагмент строки в языке Markdown выглядит следующим образом:

`Используйте if`

## Работа с цветом
**Добавили третий раздел по работе с цветом**

цвет добавляется к содержимому двумя способами:

*использовать встроенный HTML для стилей
Поскольку Markdown преобразован в HTML-код. Большинство парсеров уценки поддерживают HTML-код.*

Итак, напишите встроенный HTML-код в содержимом. Добавлен тег span со встроенными стилями для изменения цвета, веса и размера шрифта.

Ниже HTML-код добавлен в файлы (расширение .md)

<span style="color:green;font-weight:700;font-size:20px">
    markdown color font styles
</span>

Другой способ определения стилей CSS
Определите стили CSS с помощью селектора, как показано ниже.
добавить содержимое внутри тегов селектора
<style>
red { color: red }
yellow { color: yellow }
</style>

<red> red color markdown text</red>
<yellow> red color markdown text</yellow>

Сгенерированный HTML
<p><red> red color markdown text</red>
<yellow> red color markdown text</yellow></p>

*Для того чтобы добавить какой-то текст, а вернее фоновый, необходимо использовать HTML- теги таблицы*
<table>
<tr><td bgcolor="#DC143C">
Какой-то текст
</td><tr>
</table>

*А чтобы добавить цвет для текста, необходимо использовать атрибуты стилей HTML*

<a href="https://mirpozitiva.ru/wp-content/uploads/2019/11/1477469601_nature_gora.jpg" style="color:#FFA07A">Какой-то текст</a>

<p style="color:#FF4500">Слишком много новой информации, побить препода по замене!</p>
<a href="#" style="color:#FFA07A">Какой-то текст</a>


## Горячие клавиши
[ссылка] (https://www.nikomedvedev.ru/other/vscodeshortcuts/hotkeys.html все команды)



