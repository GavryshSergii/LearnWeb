##Псевдоэлементы

######Псевдоэлемент в CSS — это ключевое слово, добавляемое к селектору, которое позволяет стилизовать определённую часть выбранного элемента.

####::first-line
**`::first-line`** применяет стили к первой строке блочного элемента.

####::first-letter
**`::first-letter`** применяет стили к первой букве первой строки блочного элемента, но только если нету другого предшествующего содержимого (такого как изображения или инлайн таблицы).

- свойства, связанные с шрифтами
- свойства, связанные с фоном
- свойства для внутренних и внешних отступов
- свойства, связанные с рамкой
- свойства `color`
- свойства `text-decoration`, `text-shadow`, `text-transform`, `letter-spacing`, `word-spacing` (when appropriate), `line-height`, `text-decoration-color` (en-US), `text-decoration-line` (en-US), `text-decoration-style` (en-US), `box-shadow`, `float`, `vertical-align` (только если float равен none)

####::before
`::before` создаёт псевдоэлемент,который является первым потомком выбранного элемента.

####::after
`::after` создаёт псевдоэлемент, который является последним потомком выбранного элемента.

Часто используется для добавления косметического содержимого в элемент с помощью свойства `content`

####::-ms-clear 
доступ к кнопке обнуления поля ввода (text `<input>`)
- Internet Explorer 10 and 11 and Edge 12+

####::-moz-focus-inner 
`::-moz-focus-inner` CSS pseudo-element is a Mozilla extension that represents an inner focus ring of the <button> element as well as the button, submit, reset, and color types of the <input> element.

`.element:hover::before`


