####Примитивы:
######null
######undefined
######boolean
######number
######string
######symbol

####Непримитивы сложные
######object

####Приведение типов
#####Строковое преобразование
* требуется представление чего-либо в виде строки.
* оператор "+" со строкой является конкатенацией, а не сложением результатом будет строка
###### Явное приведение к строке String(value), на объектах   
#####Численное преобразование
* математических функциях и выражениях;
* при сравнении "=="
###### Явное приведение к числу Number(value), унарный плюс +value
#####Логическое преобразование
* if, while и т.п.
###### Явное логическое приведение Boolean(value), двойное НЕ: !!value

####Преобразовние объектов 
#####Логическое преобразование 
Любой объект - true
#####Строковое преобразование
метод Object.prototype.toString() или переопределенный метод
#####Численное преобразование
если метод valueOf переопределен, иначе toString
>непереопределенный valueOf возвращает сам объект

#####== сравнивает значение с приведением типов
#####=== сравнивает значение без приведения типов
