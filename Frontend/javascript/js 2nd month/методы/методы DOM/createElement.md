`document.createElement()` это метод JavaScript, который создает элемент DOM (Document Object Model) с заданным тегом. Например, следующий код создаст элемент `<div>`:

`let newDiv = document.createElement("div");`

Созданный элемент можно добавить в существующий документ, используя методы такие как `appendChild()` или `insertBefore()`.

`let existingDiv = document.getElementById("existing-div"); existingDiv.appendChild(newDiv);`

[[DOM В JC]]