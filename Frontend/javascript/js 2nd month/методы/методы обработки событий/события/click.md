"Click" - это событие JavaScript, которое происходит при нажатии кнопки мыши на элементе DOM. Обработчик события "click" может быть добавлен с помощью метода `addEventListener()`. Например, следующий код добавляет обработчик события "click" на элемент с идентификатором "my-button":

Copy code

`let myButton = document.getElementById("my-button"); myButton.addEventListener("click", function() {     console.log("Button clicked!"); });`

В данном примере функция-обработчик события выводит сообщение "Button clicked!" в консоль браузера при клике на кнопку.

[[addEventListener]]