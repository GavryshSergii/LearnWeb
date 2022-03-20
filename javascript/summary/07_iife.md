#IIFE (Immediately Invoked Function Expression)

#####Немедленно вызываемое функциональное выражение(Immediately Invoked Function Expression) - функциональное выражение, которое вызывается сразу же после создания.
>Это функция, которая исчезает сразу же после того как выполнится.

#####Cоздание области видимости

Любые переменные внутри IIFE не видимы для внешнего мира.

```
// Правильная IIFE
(function initGameIIFE() {
     // Весь код тут
}());
```

#####IIFE с отдаваемым значением
```
var result = (function() {
    return "From IIFE";
}());

alert(result); // alerts "From IIFE"
```
вы можете отдавать значение, которое будет назначено переменной.
#####IIFE с параметрами
```
(function IIFE(msg, times) {
    for (var i = 1; i <= times; i++) {
        console.log(msg);
    }
}("Hello!", 5));
```
##Классический модульный паттерн в JavaScript

```
var Sequence = (function sequenceIIFE() {
    
    // приватная переменная для хранения значения счетчика
    var current = 0;
    
    // объект, возвращаемый IIFE
    return {
        getCurrentValue: function() {
            return current;
        },
        
        getNextValue: function() {
            current = current + 1;
            return current;
        }
    };
    
}());

console.log(Sequence.getNextValue()); // 1
console.log(Sequence.getNextValue()); // 2
console.log(Sequence.getCurrentValue()); // 2
```
