`responseText` - это свойство объекта `XMLHttpRequest` (XHR), которое содержит ответ от сервера в виде строки.

Свойство `responseText` доступно только после того, как запрос был завершен, и его значение равно пустой строке до завершения запроса.

Например, чтобы получить ответ от сервера в виде строки, можно использовать следующий код:

`let xhr = new XMLHttpRequest(); 
`xhr.open('GET', 'http://example.com/data'); 
`xhr.onreadystatechange = function() {   
	`if (xhr.readyState === XMLHttpRequest.DONE) {  
	   console.log(xhr.responseText);   
	}
}
xhr.send();`

Здесь мы создаем новый объект XHR, открываем соединение методом GET к URL `http://example.com/data`, устанавливаем обработчик события `onreadystatechange`, который вызывается при изменении свойства `readyState`, и отправляем запрос методом `send()`. Когда `readyState` становится равным `XMLHttpRequest.DONE` (т.е. 4), выводим ответ от сервера в консоль.

Заметьте, что для получения ответа в виде строки, сервер должен отправлять ответ в формате текста (например, plain text, HTML, JSON и т.д.). Если сервер отправляет бинарные данные (например, изображения или аудио), то нужно использовать другое свойство, например, `responseType` с значением `"arraybuffer"`.

[[XmlHttpRequest]]