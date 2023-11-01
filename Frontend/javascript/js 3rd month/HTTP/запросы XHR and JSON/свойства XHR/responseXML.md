`responseXML` - это свойство объекта `XMLHttpRequest` (XHR), которое содержит ответ от сервера в виде объекта `Document`, если ответ был получен в формате XML.

Свойство `responseXML` доступно только после того, как запрос был завершен, и его значение равно `null` до завершения запроса или если ответ был получен в другом формате.

Например, чтобы получить ответ от сервера в виде объекта `Document`, можно использовать следующий код:

`let xhr = new XMLHttpRequest(); 
`xhr.open('GET', 'http://example.com/data.xml'); 
`xhr.onreadystatechange = function() {  
	`if (xhr.readyState === XMLHttpRequest.DONE) {    
	` console.log(xhr.responseXML);   
	}
}; 
xhr.send();`

Здесь мы создаем новый объект XHR, открываем соединение методом GET к URL `http://example.com/data.xml`, устанавливаем обработчик события `onreadystatechange`, который вызывается при изменении свойства `readyState`, и отправляем запрос методом `send()`. Когда `readyState` становится равным `XMLHttpRequest.DONE` (т.е. 4), выводим ответ от сервера в консоль.

Заметьте, что для получения ответа в формате XML, сервер должен отправлять ответ в формате XML и указывать соответствующий заголовок `Content-Type`. Если сервер отправляет ответ в другом формате, то свойство `responseXML` будет равно `null`.

[[XmlHttpRequest]]