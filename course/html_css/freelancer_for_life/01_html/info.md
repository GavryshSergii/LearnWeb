
#####\<html\>
`<html>` является контейнером, который заключает в себе все содержимое веб-страницы, включая теги `<head>` и `<body>`
#####\<head\>
`<head>` содержит машиночитаемую информацию (metadata) о документе, например его заголовок, скрипты и страницы стилей.
#####\<title\>
Элемент заголовка (`<title>`) определяет заголовок документа, который отображается в заголовке окна Browser или на вкладке страницы. Он содержит только текст, а теги внутри элемента игнорируются.
#####\<link\>
Ссылка на Внешний Ресурс (`<link>`) определяет отношения между текущим документом и внешним ресурсом. Этот элемент чаще всего используется для ссылки на  CSS, а также для создания иконок сайта (как для иконок в стиле "favicon", так и для иконок домашних экранов и приложений мобильных устройств) среди прочего.
#####\<meta\>
`<meta>` представляет такие Metadata, которые не могут быть представлены другими HTML-метатегами, такими как base, link, script, style или title.
#####\<style\>
`<style>` содержит стилевую информацию для документа или его части. По умолчанию стилевые инструкции внутри этого элемента считаются написанными на CSS.
#####\<body\>
`<body>` представляет собой контент (содержимое) документа HTML. В документе может быть только один элемент `<body>`.

###Строительные теги
все блочные
#####\<div\>
Элемент разделения контента HTML (`<div>`) является универсальным контейнером для потокового контента. Он не влияет на контент или макет до тех пор, пока не будет стилизован с помощью CSS.
#####\<header\>
`<header>` представляет собой вводный контент, обычно группу вводных или навигационных средств. Он может содержать другие элементы-заголовки, а также логотип, форму поиска, имя автора и другие элементы.
#####\<footer\>
`<footer>` представляет собой нижний колонтитул (футер, подвал) для своего ближайшего секционного контента или секционного корня. Футер обычно содержит информацию об авторе раздела, информацию об авторском праве или ссылки на связанные документы.
#####\<nav\>
`<nav>` определяет отдельную секцию документа, назначение которой обозначение ссылок навигации (как внутри текущего документа, так и ведущих на другую страницу). В качестве примера такой секции можно привести меню, якорные ссылки.

#####Теги заголовков \<h1\> - \<h6\>
`<h1>–<h6>` представляют собой 6 уровней заголовков секций. `<h1>` это наибольший заголовок и`<h6>`- наименьший.
- `<h1>` используется 1 раз 
- Блочные элементы.

#####\<p\>
HTML-элемент `<p>` представляет собой абзац.
- Блочный элемент.

#####\<span\>
`<span>` является основным строковым контейнером для фразового контента, который, по существу, ничего не представляет. Он может использоваться для группировки элементов в целях стилизации (использование атрибутов class или id) или потому, что они имеет общие значения атрибутов, например lang.
- строчный элемент