`setAttribute()` - это метод JavaScript, который используется для установки значения атрибута элемента HTML. Он принимает два аргумента: имя атрибута и значение атрибута.


`let element = document.getElementById("myId");
`element.setAttribute("class", "new-class");`

в этом примере, мы используем метод `getElementById` для получения элемента с id "myId", затем используем `setAttribute` для установки значения атрибута "class" на "new-class". В html это выглядит так `class = "new-class"

Это может быть также использовано для установки нового атрибута, если он еще не существует в элементе.

`let element = document.getElementById("myId");
`element.setAttribute("newattribute", "newvalue");`

Обратите внимание, что некоторые атрибуты, такие как "class" и "id", имеют специальные свойства JavaScript, которые можно использовать для получения и установки их значений, такие как `element.className` и `element.id`.

[[DOM В JC]]