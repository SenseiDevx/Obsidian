`addEventListener` - это метод JavaScript, который используется для назначения функции-обработчика на событие на определенном элементе HTML.

Обработчик событий (event handler) в JavaScript - это функция, которая вызывается, когда определенное событие происходит на элементе HTML. Например, функция может быть назначена как обработчик события "click" для кнопки, и выполняется код внутри функции, когда кнопка нажимается.

Метод `addEventListener` используется для назначения обработчика события на элемент. Этот метод принимает три аргумента: имя события, функцию-обработчик и опциональный объект опций.

Этот метод принимает три аргумента: имя события, функцию-обработчик и опциональный объект опций.


`let element = document.getElementById("myId"); element.addEventListener("click", myFunction);  function myFunction() {     console.log("The button was clicked!"); }`


[[метод оброботки событий]]