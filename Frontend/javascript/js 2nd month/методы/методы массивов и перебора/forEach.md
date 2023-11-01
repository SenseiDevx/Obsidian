`forEach()` - это метод массива в JavaScript, который позволяет вам выполнить функцию для каждого элемента массива. Он принимает в качестве аргумента коллбек-функцию, которая будет вызвана для каждого элемента массива. forEach особо то и не отличается от map, в отличии от map forEach не создает новый массив он просто изменяет только тот же массив

`forEach()` - это метод JavaScript, который позволяет перебрать каждый элемент массива и выполнить над ним определенную функцию.

Пример 1:
`let numbers = [1, 2, 3, 4, 5];
`numbers.forEach(function(number) {  
`console.log(number); });`

Этот код выведет в консоль каждое число из массива numbers.

Пример 2:
`let names = ['John', 'Jane', 'Mike', 'Mary']; 
`names.forEach(function(name, index) { 
`console.log(index + 1 + '. ' + name); });`
Этот код выведет в консоль имена из массива names с нумерацией индекса.

Пример 3:
`let shoppingList = ['milk', 'bread', 'eggs', 'coffee']; 
`shoppingList.forEach(function(item) {  
`console.log("Don't forget to buy " + item + "."); });`
Этот код выведет в консоль напоминание о каждом элементе из массива shoppingList.

Пример 4:
`let numbers = [1, 2, 3, 4, 5]; 
`numbers.forEach(function(number, index, array) {   
`array[index] = number * 2; }); console.log(numbers);`
Этот код удваивает каждое число в массиве numbers и выводит новый массив в консоль.

[[методы массивов в jc]]