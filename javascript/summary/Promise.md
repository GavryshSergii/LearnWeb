Промис (Promise) - объект

У промиса есть 3 состояния:
1. Промис в состоянии ожидания (pending). Когда вы не знаете, получите ли вы мобильный телефон к следующей неделе или нет.

2. Промис решен (resolved). Вам реально купят новый телефон.

3. Промис отклонен (rejected). Вы не получили новый мобильный телефон, так как всё-таки, мама была не в настроении.
```
/_ ES5 _/
var isMomHappy = false;

// Promise
var willIGetNewPhone = new Promise(
    function (resolve, reject) {
        if (isMomHappy) {
            var phone = {
                brand: 'Samsung',
                color: 'black'
            };
            resolve(phone); // Всё выполнено
        } else {
            var reason = new Error('mom is not happy');
            reject(reason); // reject
        }

    }
);

// Вызываем промис
var askMom = function () {
    willIGetNewPhone
        .then(function (fulfilled) {
            // yay, you got a new phone
            console.log(fulfilled);
         // output: { brand: 'Samsung', color: 'black' }
        })
        .catch(function (error) {
            // oops, mom don't buy it
            console.log(error.message);
         // output: 'mom is not happy'
        });
};

askMom();
```
