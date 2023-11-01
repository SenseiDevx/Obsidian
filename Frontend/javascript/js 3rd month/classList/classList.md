 classList - это свойство объекта элемента в DOM (Document Object Model) в JavaScript, которое предоставляет методы для добавления, удаления, переключения классов CSS элемента.

Свойство classList возвращ ает объект DOMTokenList, который содержит все классы элемента в виде отдельных токенов. Этот объект предоставляет следующие методы:

-   add(className) - добавляет класс className в список классов элемента.
-   remove(className) - удаляет класс className из списка классов элемента.
-   toggle(className) - переключает наличие класса className. Если класс уже существует, он будет    удален, если его нет, он будет добавлен.
-   contains(className) - проверяет, есть ли класс className в списке классов элемента.

Вот пример использования свойства classList:

`// получаем элемент по id var element = document.getElementById("my-element"); 
``// добавляем класс  active
``"active" element.classList.add("active"); 

``// удаляем класс "inactive" 
`element.classList.remove("inactive");  

``// переключаем класс "selected" 
`element.classList.toggle("selected"); 

``// проверяем, есть ли класс "hidden" 
`var isHidden = element.classList.contains("hidden");`

С помощью свойства classList можно легко изменять классы элементов в DOM, что делает его очень полезным при разработке веб-приложений и интерфейсов.
[[DOM В JC]]