###Отступы размеры характеристики

#####padding
Внутренний отступ элемента. 
При указании поля в процентах, значение считается от ширины родителя элемента.
Свойство не наследуется.

- `padding: со_всех_сторон`;
- `padding: сверху справа снизу слева`;
- `padding: сверху_снизу справа_слева`;
- `padding: сверху справа_слева снизу`;

+ Отступ сверху и снизу не действует на срочные теги

#####margin
Внешний отступ элемента. 
При указании поля в процентах, значение считается от ширины родителя элемента.
Свойство не наследуется.
Значение может быть как положительным, так и отрицательным числом.

- `margin: со_всех_сторон`;
- `margin: сверху справа снизу слева`;
- `margin: сверху_снизу справа_слева`;
- `margin: сверху справа_слева снизу`;

+ Отступ сверху и снизу не действует на срочные теги

#####width
Устанавливает ширину блочных тегов и некоторыйх строчных (например img).
Свойство не наследуется.
- `width:100px`;
- `width:10%`;

#####max-width
Устанавливает максимальную ширину блочных тегов и некоторыйх строчных (например img)

#####min-width
Устанавливает минимальную ширину блочных тегов и некоторыйх строчных (например img)

#####height:
Устанавливает высоту блочных тегов и некоторыйх строчных (например img)
Свойство не наследуется.
- `height:100px`;
- `height:10%`;

#####min-height
Свойство не наследуется.

#####max-height
Свойство не наследуется.

#####overflow 
Управляет отображением содержания блочного элемента
- `visible` - Отображается все содержание элемента, даже за пределами установленной высоты и ширины. 
- `hidden` - Отображается только область внутри элемента, остальное будет скрыто.
- `scroll` - Всегда добавляются полосы прокрутки.
- `auto` - Полосы прокрутки добавляются только при необходимости.

#####display:
Многоцелевое свойство, которое определяет, как элемент должен быть показан в документе.
Свойство не наследуется.

- `block` - Элемент показывается как блочный. Применение этого значения для встроенных элементов, например тега `<span>`, заставляет его вести подобно блокам — происходит перенос строк в начале и в конце содержимого. 											
- `inline` - Элемент отображается как встроенный. Использование блочных тегов, таких как `<div>` и `<p>`, автоматически создает перенос и показывает содержимое этих тегов с новой строки. Значение `inline` отменяет эту особенность, поэтому содержимое блочных элементов начинается с того места, где окончился предыдущий элемент. 											
- `inline - block` - Это значение генерирует блочный элемент, который обтекается другими элементами веб-страницы подобно встроенному элементу. Фактически такой элемент по своему действию похож на встраиваемые элементы (вроде тега `<img>`). При этом его внутренняя часть форматируется как блочный элемент, а сам элемент — как встроенный. 											
- `none` - Временно удаляет элемент из документа. Занимаемое им место не резервируется и веб-страница формируется так, словно элемента и не было. 

#####box-sizing
Применяется для изменения алгоритма расчета ширины и высоты элемента. 
Свойство наследуется.
- `content-box` - Основывается на стандартах CSS, при этом свойства width и height задают ширину и высоту контента и не включают в себя значения отступов, полей и границ.
- `border-box` - Свойства **_width_** и **_height_** включают в себя значения полей и границ, но не отступов (`margin`). Эта модель используется браузером Internet Exporer в режиме несовместимости.
- `padding-box` - Свойства **_width_** и **_height_** включают в себя значения полей, но не отступов (`margin`) и границ (`border`). 


###Свойства оформления
#####border
Универсальное свойство **_border_** позволяет одновременно установить толщину, 
стиль и цвет границы вокруг элемента.
- `border: 1px solid #000; (размер стиль цвет)`
Основные стили:
- `solid`
- `dotted`
- `dashed`

#####border-radius
Устанавливает радиус скругления уголков блока.
- `border-radius:50%;` - круг
Можно использовать вместе с `overflow: hidden;`

#####outline
Универсальное свойство, одновременно устанавливающее цвет, 
стиль и толщину внешней границы на всех четырех сторонах элемента. 
В отличие от линии, задаваемой через border, свойство **_outline_** 
не влияет на положение блока и его ширину. 
Также нельзя задать параметры линии на отдельных сторонах элемента, 
**_outline_** применяется сразу ко всем четырём сторонам. 

#####box-shadow
Добавляет тень к элементу.
`box-shadow: сдвиг_по_гориз сдвиг_по_верт радиус расстояние цвет`
- `box-shadow: 5px 5px 10 px 5px #000`
- `box-shadow: inset 5px 5px 10 px 5px #000` - тень внутрь блока
Можно добавить много теней. На тень влияет свойство **_border-radius_**.

#####opacity
Определяет уровень прозрачности элемента.
Отличие **_opacity:0;_** от **_display:none;_** в том что блок не убирается из верстки а только становиться прозрачным, то есть занимаемое им место остается. Так же, с прозрачными элементами все еще можно взаимодействовать, например кликать по ссылкам.

#####visibility
Предназначен для отображения или скрытия элемента.
Отличие **_visibility: hidden;_** от **_display:none;_** в том что блок не убирается из верстки а только скрывается, то есть занимаемое им место остается.
Отличие **_visibility: hidden;_** от **_opacity:0;_** в том что блок скрывается и взаимодействовать с ним нельзя.

###Background


#####background:
Универсальное свойство background позволяет установить одновременно несколько характеристик фона а именно:

#####background-color - Определяет цвет фона элемента.

#####background-image - Устанавливает фоновое изображение для элемента.

Так же значением свойства можно указать градиент:
линейный:
`background:linear-gradient(to top, #fefcea, #f1da36); `
радиальный:
`background:radial-gradient(ellipse at center, rgba(30,87,153,1) 0%,rgba(41,137,216,1) 50%,rgba(32,124,202,1) 51%,rgba(125,185,232,1) 100%);`

Подробнее о градиентах:
http://htmlbook.ru/css3-na-primerakh/lineinyi-gradient

Инструмент создания готового кода:
https://www.colorzilla.com/gradient-editor/

#####background-position - Задает начальное положение фонового изображения, установленного с помощью свойства background-image.

#####background-repeat - Определяет, как будет повторяться фоновое изображение, установленное с помощью свойства background-image.
no-repeat -  Устанавливает одно фоновое изображение в элементе без его повторений, положение которого определяется свойством background-position (по умолчанию в левом верхнем углу). Аналогично no-repeat no-repeat.
repeat - Фоновое изображение повторяется по горизонтали и вертикали. Аналогично repeat repeat.
repeat-x - Фоновый рисунок повторяется только по горизонтали. Аналогично repeat no-repeat.
repeat-y - Фоновый рисунок повторяется только по вертикали. Аналогично no-repeat repeat.
inherit -Наследует значение родителя.
space - Изображение повторяется столько раз, чтобы полностью заполнить область; если это не удаётся, между картинками добавляется пустое пространство.
round - Изображение повторяется так, чтобы в области поместилось целое число рисунков; если это не удаётся сделать, то фоновые рисунки масштабируются.

#####background-attachment - Устанавливает, будет ли прокручиваться фоновое изображение вместе с содержимым элемента.
fixed - Делает фоновое изображение элемента неподвижным. 
scroll - Позволяет перемещаться фону вместе с содержимым.
inherit - Наследует значение родителя.
local - Фон фиксируется с учётом поведения элемента. Если элемент имеет прокрутку, то фон будет прокручиваться вместе с содержимым, но фон выходящий за рамки элемента остаётся на месте.

#####background-size  - Масштабирует фоновое изображение согласно заданным размерам.
<значение> - Задает размер в любых доступных для CSS единицах. 
<проценты> - Задает размер фоновой картинки в процентах от ширины или высоты элемента. 
auto - Если задано одновременно для ширины и высоты (auto auto), размеры фона остаются исходными; если только для одной стороны картинки (100px auto), то размер вычисляется автоматически исходя из пропорций картинки.
cover - Масштабирует изображение с сохранением пропорций так, чтобы его ширина или высота равнялась ширине или высоте блока.
contain - Масштабирует изображение с сохранением пропорций таким образом, чтобы картинка целиком поместилась внутрь блока. 
Если установлено одно значение, оно задает ширину фона, второе значение принимается за auto. Пропорции картинки при этом сохраняются. Использование двух значений через пробел задает ширину и высоту фоновой картинки.

Свойство background позволяет задать несколько изображений через запятую, 
причем со своими настройками позиционарования маштабирования и прокрутки
