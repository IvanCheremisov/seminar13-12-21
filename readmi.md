# Инструкция по работе с Git


## Основные команды Git
### Создание локального репозитория
Создать локальный репозиторий можно с помощью команды *idit init* для этого команда должна применяться в той папке, где будет репозиторий.

### Добавление файлов в репозиторий 
Версионность  к файлу добавляется с помощью команды *git add*. Команда применяется следующим образом: *git add <название файла> *.

### Создание комита 
Для того , что бы создать новый коммит необходимо использовать команду *git commit*. Применяется она следующим образом: *git commit -m"<сообщение к коммиту>"*. Сообщение коммиту писать ***ОБЯЗАТЕЛЬНО***.

### Просмотр наличия изменений
Для того, чтобы посмотреть имеются ли изменения в локальном репозитории используется команда *git status*. Достаточно ее просто применить в пепке с препозиторием.

### Просмотр разницы между текущей версией и последней  "сохраненной"
Для того, чтобы посмотреть разницу между последним и текущей версией файлов, используется команда *git diff*. Достаточно ее применть в папке с репозиторием.

### Просмотр истории коммитов 
Для просмотра истории комитов используется команда *git log*. Для того, чтобы увидеть историю коммитов, достаточно просто применить эту команду в папке с репозиторием.

### Перемещение между изменениями 
Для того, чтобы переместиться на какое-то из прошлых изменений необходимо использовать команду *git checkaut*. Применяется она следующим образом в папке с репозиторием: *git checkout <номер коммита>*. Для возврата к последему коммиту ветки нужно использовать команду *git checkout master*.

### Просмотр различий двух деревьев
Команда *git difftool* просто запускает внешнюю утилиту сравнения для показа различий в двух деревьях, на случай если вы хотите использовать что-либо отличное от встроенного просмотрщика *git diff*.

### Отмена индексации файла
Команда *git reset*, как можно догадаться из названия, используется в основном для отмены изменений. Она изменяет указатель HEAD и, опционально, состояние индекса. Также эта команда может изменить файлы в рабочем каталоге при использовании параметра *--hard*, что может привести к потере наработок при неправильном использовании, так что убедитесь в серьёзности своих намерений прежде чем использовать его.

### Удаление файлов 
Команда *git rm* используется в Git для удаления файлов из индекса и рабочей копии. Она похожа на *git add* с тем лишь исключением, что она удаляет, а не добавляет файлы для следующего коммита.

### Перемещение файлов 
Команда *git mv* - это всего лишь удобный способ переместить файл, а затем выполнить *git add* для нового файла и *git rm* для старого.
### Отчистка рабочего каталога 
Команда *git clean* используется для удаления мусора из рабочего каталога. Это могут быть результаты сборки проекта или файлы конфликтов слияний.

# Инструкция по работе с Markdown

##  ___Блочные элементы___
## Параграфы и разрывы строк
Для того, чтобы создать параграф с использованием синтаксиса языка Markdown, достаточно отделить строки текста одной (или более) пустой строкой (пустой считается всякая строка, которая не содержит в себе ничего, кроме пробелов и символов табуляции). Для того, чтобы вставить видимый перенос строки (элемент <br/>) необходимо окончить строку двумя пробелами и нажатием клавиши «Enter».

## Заголовки 
Язык разметки Markdown поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом (#). Выделение заголовков с помощью подчеркивания производится знаками равенства (=) в случае, если заголовок первого уровня, и дефисами (-) в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается. При выделении заголовков с помощью символа (#) используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами (#), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.

### __Заголовки первого и второго уровней, выполненные с помощью подчеркивания, выглядят следующим образом:__
Заголовок первого уровня
=
Заголовок второго уровня
-
### __Заголовки первого, второго, третьего, четвертого, пятого и  шестого уровней, выполненные с помощью символа (#), выглядят следующим образом:__
#  Заголовок первого уровня
## Заголовок первого уровня
### Заголовок третьего уровня
#### Заголовок шестого уровня
##### Заголовок первого уровня
###### Заголовок первого уровня

### __Приведенные выше заголовки, выполненные с помощью символа (#) тождественны следующим:__

#  Заголовок первого уровня #
### Заголовок третьего уровня ###
###### Заголовок шестого уровня ######

## Цитаты 
Для обозначения цитат в языке Markdown используется знак «больше» (>). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования (>). Цитаты в Markdown могут содержать всевозможные элементы разметки. Цитаты в языке Markdown выглядят следующим образом:

>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

>Это пример цитаты,
в которой угловая скобка
ставится только перед началом нового параграфа.
>Второй параграф.
### __Вложение цитаты в цитату выглядит следующим образом:__
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования

## Списки 
Markdown поддерживает упорядоченные (нумерованные) и неупорядоченные (ненумерованные) списки. Для формирования неупорядоченный списков используются такие маркеры, как звездочки (*), плюсы (+) и дефисы(-). Все перечисленные маркеры могут использоваться взаимозаменяемо. Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны, так как они не оказывают влияния на выходной HTML код. Как бы ни нумеровал пользователь список, на выходе он в любом случае будет иметь упорядоченный список, начинающийся с единицы (1, 2, 3…). Эту особенность стоит учитывать в том случае, когда необходимо использовать порядковые номера элементов в списке, чтобы они соответствовали номерам, получающимся в HTML. Упорядоченные списки всегда следует начинать с единицы. Маркеры списков обычно начинаются с начала строки, однако они могут быть сдвинуты, но не более чем на 3 пробела. За маркером должен следовать пробел, либо символ табуляции. При необходимости в список можно вставить цитату. В этом случае обозначения цитирования ( «>» ) нужно писать с отступом. 

__Упорядоченные списки выглядят следующим образом:__
1.	Опанька
2.	Опаньки
3.	Опаньке

__Неупорядоченные списки выглядят следующим образом:__
* Опанька
* Опаньки
* Опаньке

__Или:__
- Опанька
- Опаньки
- Опаньке

__Или__
+ Опанька
+ Опаньки
+ Опаньке

__Цитата, вставленная в список, выглядит следующим образом:__
1. Элемент списка с цитатой:

    > Это цитата
    > внутри элемента списка.

 2. Элемент списка с цитатой

 При вставке цитат в элементы списка важно учитывать, что элементы списка должны находиться на одном уровне, а цитаты должны указываться с отступом. В случае, если правило с единым уровнем списка не соблюдается, следующий после цитаты элемент списка будет автоматически нумероваться цифрой «1.». Кроме того, при необходимости в список можно вставить исходный код. В этом случае его нужно писать с двойным отступом – 8 пробелов или 2 символа табуляции.

 + __Элемент списка, содержащий исходный код.__

       <исходный код > 

 ## Блоки кода 
 Отформатированные блоки кода используются в случае необходимости процитировать исходный код программ или разметки. Для создания блока кода в языке Markdown необходимо каждую строку параграфа начинать с отступа, состоящего из четырех пробелов или одного символа табуляции. Блок кода продолжается до тех пор, пока не встретится строка без отступа (или конец текста). Внутри блока кода амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в элементы HTML разметки. Кроме того, следует отметить, что внутри блоков кода обычный синтаксис Markdown не обрабатывается. Блок кода в Markdown выглядит следующим образом:

 __Это обычный параграф:__
 
    Это блок кода

## Горизонтальные линии (разделители)

Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы.

__Горизонтальные линии в Markdown выглядят следующим образом:__

Первая часть текста, который необходимо разделить
***
Вторая часть текста, который необходимо разделить

__Или:__

Первая часть текста, который необходимо разделить

---

Вторая часть текста, который необходимо разделить

При использовании данного инструмента важно помнить, что после первой части текста и перед второй необходимо оставлять пустую строку. Данное правило необходимо соблюдать только при использовании дефисов. Если его не соблюдать, на экран будет выведен заголовок второго уровня и строка обычного текста. При использовании символа звездочки данным правилом можно пренебречь.

## ___Строчные элементы___

## Ссылки

Markdown поддерживает два стиля оформления ссылок:

+ Гиперссылка, с немедленным указанием адреса (внутритекстовая);
+ Гиперссылка, подобная сноске.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

    [например](https://thumb.cloud.mail.ru/thumb/xw1/DSC_0191-1.jpg)

 __При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).__

     [пример][id]:
__Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок:__

    [пример] [id]:

__В этом случае возможно определить идентификатор в любом месте документа:__ 
     
    [id]: https://thumb.cloud.mail.ru/thumb/xw1/DSC_0191-1.jpg

__Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:__

    [текст ссылки][a]
    [текст ссылки][A]

 Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется и в качестве её имени, а вторая пара квадратных скобок остаётся пустою. Например, чтобы сделать слово «coffee» гиперссылкой, ведущей на сайт http://coffee.com/, достаточно написать:
      
    [coffee][]

__и затем определить гиперссылку:__

    [coffee]: http://coffee.com/

## Выделение текста

Markdown воспринимает звёздочки «*» и символы подчёркивания «_» как признаки смыслового выделения текста. Иными словами, текст, окруженный одинарными символами, выделяется курсивным шрифтом, а текст, окруженный двойными символами, выделяется полужирным шрифтом. Также, выделенный фрагмент может находиться в любой части слова. Текст, выделенный курсивом с использованием синтаксиса языка Markdown, выглядит следующим образом:

 *Опаньки* 

Текст, выделенный полужирным шрифтом с использованием синтаксиса языка Markdown, выглядит следующим образом:

**Опаньки**

Текст, выделенный курсивным полужирным шрифтом с использованием синтаксиса языка Markdown выглядит следующим образом:

***Опаньки***

Все приведенные выше примеры аналогичны следующим:

_Опаньки_

__Опаньки__

Пере___опаньки___опа

___Опаньки___  

## Кодовые фрагменты строк

Чтобы отметить фрагмент строки, содержащий код, необходимо окружить его обратными апострофами «`». При использовании кодовых фрагментов строк текст будет отображаться в виде моноширинного шрифта. В отличие от блоков кода, кодовый фрагмент позволяет поместить код внутрь обычного абзаца текста. Кодовый фрагмент строки в языке Markdown выглядит следующим образом:

Используйте оператор `if`

## Изображения

В Markdown существует 2 способа вставки изображений в документ:

__С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:__ 

    ![Альтернативный текст](/путь/к/изображению.jpg)

__Или:__

    ![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")

Иными словами, он состоит из следующих элементов:
- восклицательный знак;
- квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
- круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.

__С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:__

    ![Альтернативный текст][id]

где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

    [id]: путь/к/изображению "Необязательная подсказка"

Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).

## Дополнительные элементы

__Обратный слеш__

Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении. Полный список данных символов приводится ниже:

«\» - слеш;

«`» - обратный апостроф;

«*» - звездочка;

«_» - символ подчеркивания;

«{}» - фигурные скобки;

«[]» - квадратные скобки;

«()» - круглые скобки;

«#» - символ решетки;

«+» - плюс;

«-» - минус (дефис);

«.» – точка;

«!» - восклицательный знак.

## Автоматические ссылки

Markdown поддерживает упрощённый порядок автоматического создания ссылок для URL-адресов и адресов электронной почты. Для этого достаточно поместить URL-адрес или почтовый адрес в угловые скобки, и Markdown сделает его гиперссылкой. В отличие от вышеописанных стилей, в данном случае сам же URL-адрес или почтовый адрес становится и текстом гиперссылки. Автоматические ссылки на адреса электронной почты работают аналогично. Автоматические ссылки в языке Markdown выглядят следующим образом:

    <http://coffee.com/>

Автоматическая ссылка на адрес электронной почты в Markdown выглядит следующим образом:

    <address@coffee.com>

## Специальные символы __HTML__

В языке HTML существует два символа, требующих специального рассмотрения: это символы («<») и («&»). Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения специального символа HTML. Для того чтобы использовать эти символы в их буквальном смысле, необходимо заменить их элементами HTML, а именно &lt; и &amp; соответственно. При использовании Markdown подобных действий совершать не нужно. Он позволяет использовать эти символы в исходном виде. В случае если амперсанд используется как часть спецсимвола HTML, он останется неизменным. В противном случае Markdown преобразует его в &amp;.


Отличная работа.

Итог: 5+