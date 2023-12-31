`Promise` - это объект в JavaScript, который представляет результат асинхронной операции, которая может быть завершена успешно (resolve) или с ошибкой (reject).

_Промисификация_ – это когда берут асинхронную функциональность и делают для неё обёртку, возвращающую промис.
После промисификации использование функциональности зачастую становится гораздо удобнее.

Промисы (promises) в JavaScript - это объекты, которые представляют собой асинхронную операцию и используются для управления ее результатом.

С помощью `Promise` можно создавать асинхронный код в JavaScript, который более удобен и понятен, чем использование колбек-функций.

`Promise` имеет три состояния:

-   `pending` (ожидание) - начальное состояние, когда `Promise` создан, но его значение еще неизвестно.
-   `fulfilled(resolved)` (выполнено) - когда асинхронная операция завершилась успешно и вернула результат.
-   `rejected` (отклонено) - когда асинхронная операция завершилась с ошибкой.

Создание `Promise`:

`const promise = new Promise((resolve, reject) => {   // асинхронная операция  
		`if (успешно выполнено) {     
		`resolve(result); // вернуть результат   
		`} else {     reject(error); // вернуть ошибку   
`} });`

Здесь `resolve` - функция, вызываемая в случае успешного выполнения операции, и передающая ей результат. `reject` - функция, вызываемая в случае ошибки и передающая ей ошибку.

`Promise` имеет методы для работы с его состоянием и результатом:

-   `then()` - вызывается при успешном выполнении операции и получает результат в качестве параметра.
-   `catch()` - вызывается при ошибке и получает ошибку в качестве параметра.
-   `finally()` - вызывается в любом случае после завершения операции, в том числе и при ошибке.

Например:

``const promise = new Promise((resolve, reject) => { 
	`setTimeout(() => {     
		`const randomNumber = Math.random();    
			` if (randomNumber > 0.5) {      
			` resolve(randomNumber);     
			`} else {       reject(new Error('Число меньше 0.5')); 
			`}   }, 1000); });  promise   
			`.then(result => console.log(`Результат: ${result}`))  
			` .catch(error => console.error(error.message))   
			`.finally(() => console.log('Операция завершена'));``

Здесь мы создаем `Promise`, который возвращает случайное число, и вызываем методы `then()`, `catch()` и `finally()` для его обработки. Если число больше 0.5, метод `then()` будет вызван, иначе - метод `catch()`. `finally()` будет вызван в любом случае после завершения операции.

[[Frontend/javascript/js 3rd month/ассинхронность/promise/fetch]]