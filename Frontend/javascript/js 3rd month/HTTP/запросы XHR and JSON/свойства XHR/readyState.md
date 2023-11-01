`readyState` - это свойство объекта `XMLHttpRequest` (XHR), которое содержит текущее состояние XHR-запроса.

Свойство `readyState` может принимать следующие значения:

-   `0` (UNSENT) - XHR-запрос не был инициализирован методом `open()`.
-   `1` (OPENED) - XHR-запрос был инициализирован, но метод `send()` не был вызван.
-   `2` (HEADERS_RECEIVED) - XHR-запрос был отправлен, и сервер прислал заголовки ответа.
-   `3` (LOADING) - XHR-запрос находится в процессе загрузки ответа.
-   `4` (DONE) - XHR-запрос завершен, и ответ полностью загружен.

Например, можно использовать следующий код, чтобы отслеживать изменения свойства `readyState` в процессе выполнения запроса:

`let xhr = new XMLHttpRequest(); 
`xhr.open('GET', 'http://example.com/data'); 
`xhr.onreadystatechange = function() { 
	`if (xhr.readyState === XMLHttpRequest.DONE) {  
	` console.log('Запрос завершен');    
	`console.log('Статус ответа:', xhr.status);   
	` console.log('Текст ответа:', xhr.responseText);   } }; xhr.send();`

Здесь мы создаем новый объект XHR, открываем соединение методом GET к URL `http://example.com/data`, устанавливаем обработчик события `onreadystatechange`, который вызывается при изменении свойства `readyState`, и отправляем запрос методом `send()`. Когда `readyState` становится равным `XMLHttpRequest.DONE` (т.е. 4), выводим сообщение в консоль и печатаем статус и текст ответа.
[[XmlHttpRequest]]