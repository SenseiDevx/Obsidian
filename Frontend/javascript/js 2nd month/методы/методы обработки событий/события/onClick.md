`onclick` - это свойство JavaScript, которое предоставляет короткий способ назначить обработчик события "click" на элементе DOM. Это свойство принимает функцию, которая будет вызвана при нажатии кнопки мыши на элементе.

Например, следующий код добавляет обработчик события "click" на элемент с идентификатором "my-button":

Copy code

`let myButton = document.getElementById("my-button"); myButton.onclick = function() {     console.log("Button clicked!"); };`

В данном примере функция-обработчик события выводит сообщение "Button clicked!" в консоль браузера при клике на кнопку.

[[addEventListener]]