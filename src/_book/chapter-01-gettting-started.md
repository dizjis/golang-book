---
title:  "Приступая к работе"
layout: "chapter"

---

Программирование — это исскуство, ремесло и наука о написании программ, определяющих то, как компьютер будет работать. Эта книга научит вас писать компьютерные программы, используя язык программирования, разработанный в компании Google, под названием Go.

Go — язык общего назначения с широкими возможностями и понятным синтаксисом. Благодаря мультиплатформенности, надежной, хорошо документированной стандартной библиотеке и ориентированности на удобные подходы к самой разработке, Go является идеальным языком для первых шагов в программировании.

Процесс разработки приложений на Go (и на большинстве других языков программирования) довольно прост:

* сбор требований,
* поиск решения,
* написание кода, реализующего решения,
* компиляция кода в исполняемый файл,
* запуск и тестирование программы.

Процесс этот итеративный (то есть повторяющийся много раз) и шаги, как правило, совпадают. Но прежде чем мы напишем нашу первую программу на Go, нужно понять несколько основных принципов.

## Файлы и директории

Файл представляет собой набор данных, хранящийся в блоке с определенным именем. Современные операционные системы (такие как Windows или Mac OSX) содержат миллионы файлов, содержащих большой объем различной информации — начиная от текстовых документов заканчивая программами и мультимедиа-файлами.

Файлы определенным образом храняться в компьютере: все они имеют имя, определенный размер (измеряемый в байтах) и соответствующий тип. Обычно тип файла определяется по его расширению — части имени, которая стоит после последней `.`. Например, файл названный `hello.txt` имеет расширение `txt`, значит содержит текстовую информацию.

Папки (так же называемые директориями) используются для группирования нескольких файлов.

## Терминал

Большая чась взаимодействия с компьютером сейчас осуществляется с помощью графического пользовательского интерфейса (GUI). Мы используем клавиатуру, мышь, сенсорные экраны для взаимодействия с визуальными кнопками и другими отображаемыми элементами.

Но так было не всегда. Перед GUI в ходу был терминал — простой текстовый интерфейс к компьютеру, где вместо работы с кнопками на экране мы вводили команды и получали ответы.

И хотя может показаться, что большая часть компьютерного мира оставила терминал далеко позади как пережиток прошлого, правда в том, что терминал всё еще остаётся фундаментальным пользовательским интерфейсом, используемым большинством языков программирования на большинстве компьютеров. Go не исключение, поэтому прежде чем писать программу на Go, понадобится элементарное понимание того, как работает терминал.

### Windows

Чтобы вызвать терминал (командную строку) в Windows, нужно нажать комбинацию клавишь Win+R (удерживая клавишу со логотипом Windows нажмите R), ввести в появившееся окно `cmd.exe` и нажать Enter. Вы должны увидеть черное окно, похожее на то, что ниже:

![](/img/chapter-01/01.png)

По умолчанию, командная строка запускается из вашей домашней директории (в моём случае это `C:\Users\caleb`). Вы отдаёте команды компьютеру, набирая их в этом окне и нажимая Enter. Попробуйте ввести команду `dir`, которая выводит содержимое текущего каталога на экран. Вы должны увидеть что-то вроде этого:

    C:\Users\caleb>dir
    Volume in drive C has no label.
    Volume Serial Number is B2F5-F125

Вы можете изменить текущий каталог с помощью команды `cd`. Например, там наверняка есть директория под названием `Desktop`. Вы можете посмотреть её содержимое набрав `cd Desktop`, а затем `dir`. Чтобы вернуться в домашнюю директорию, используйте специальное имя `..` (две точки): `cd ..`. Одна точка обозначает текущий каталог (известен как рабочая директоия), так что `cd .` ничего не сделает. Конечно, существует намного больше команд, которые можно использовать, но этих будет вполне достаточно для начала.

### OSX

В OSX терминал можно найти перейдя в Finder → Applications → Utilities → Terminal. Вы увидите такое окно:

![](/img/chapter-01/02.png)

По умолчанию, командная строка запускается из вашей домашней директории (в моём случае это `/Users/caleb`). Вы отдаёте команды компьютеру, набирая их в этом окне и нажимая Enter. Попробуйте ввести команду `ls`, которая выводит содержимое текущего каталога на экран. Вы должны увидеть что-то вроде этого:

    caleb-min:~ caleb$ ls
    Desktop      Downloads      Movies     Pictures
    Documents    Library        Music      Public

Вы можете изменить текущий каталог с помощью команды `cd`. Например, там наверняка есть директория под названием `Desktop`. Вы можете посмотреть её содержимое набрав `cd Desktop`, а затем `ls`. Чтобы вернуться в домашнюю директорию, используйте специальное имя `..` (две точки): `cd ..`. Одна точка обозначает текущий каталог (известен как рабочая директоия), так что `cd .` ничего не сделает. Конечно, существует намного больше команд, которые можно использовать, но этих будет вполне достаточно для начала.