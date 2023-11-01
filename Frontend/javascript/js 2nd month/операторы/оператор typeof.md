Оператор `typeof` в JavaScript возвращает строку, указывающую тип значения, которое находится справа от него. Он может использоваться для проверки типа значений в условных операторах или для отладки.

Примеры использования:

`console.log(typeof 123); // "number" 
`console.log(typeof 'hello'); // "string" 
`console.log(typeof true); // "boolean" 
`console.log(typeof { a: 1 }); // "object"
`console.log(typeof [1, 2, 3]); // "object" (в некоторых реализациях JavaScript возвращает "array") 
`console.log(typeof null); // "object"
`console.log(typeof undefined); // "undefined" 
`console.log(typeof function() {}); // "function"`

Обратите внимание, что оператор `typeof` может возвращать строку "object" для объектов и массивов. Для точной проверки типа объекта или массива следует использовать специальные функции: `Array.isArray()` и `Object.prototype.toString.call()`.


[[операторы в jc]]