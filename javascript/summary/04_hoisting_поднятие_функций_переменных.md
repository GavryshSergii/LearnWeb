#Поднятие (hoisting) функций и переменных
поднимаются (hoisting) или другими словами «перемещаются» в начало текущего контекста.


######Function declaration можно использовать в JavaScript до их объявления.
######Поднимается так же объявление переменных объявленных с помощью ключевого слова var (только объявление без инициализации)
Переменные объявленные с помощью ключевых слов **let** и **const** не подвержены hoisting 
 
Function declaration

`function greet() {
  console.log('Привет!');
}` 

Function expression

`const greet = function () {
  console.log('Привет!');
}
` 
