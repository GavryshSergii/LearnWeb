## Замыкание (Closures)

######Замыкание — это функция, захватывающая лексическое окружение того контекста, где она создана. В дальнейшем это окружение используется для разрешения идентификаторов. 
* Захваченное окружение переживает порождающий ее контекст. 
* Если бы не было замыкания, активационное окружение функции было бы уничтожено. Однако функция его захватила, и поэтому оно не может быть удалено, и сохраняется — для обеспечения семантики статической области видимости.


Функции в ECMAScript являются объектами первого класса (first-class objects).
######Функция первого класса — функция, которая может быть использованна в качестве обычных данных: т.е. сохранена в переменную, передана в качестве аргумента, или возвращена в качестве значения из другой функции.
######Свободная переменная — переменная, не являющаяся ни параметром, ни локальной переменной данной функции.
######Статическая область видимости также называется лексической областью видмости (lexical scope) — язык программирования использует статическую область видимости, если только по анализу исходного кода, можно определить, в каком лексическом окружении будут разрешены свободные переменные.


**Нисходящая фунарг-проблема**, т.е. неоднозначность, возникающая при определении правильного лексического окружения свободной переменной: должно ли это быть окружение времени создания, или же окружение времени вызова?

Данная проблема решена соглашением использования статической области видимости (static scope), т.е. окружения времени создания.

**Восходящая фунарг-проблема**. Единственное отличие здесь в том, что захваченное окружение переживает порождающий ее контекст.

Если бы не было замыкания, активационное окружение функции было бы уничтожено. Однако мы его захватили, и поэтому оно не может быть удалено, и сохраняется — для обеспечения семантики статической области видимости.

Технический механизм нисходящего и восходящего фунарга абсолютно идентичен, и является механизмом статической области видимости.
