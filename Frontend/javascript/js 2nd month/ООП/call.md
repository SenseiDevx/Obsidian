`call()` - это метод JavaScript, который позволяет вызывать функцию с определенным контекстом выполнения и аргументами. Это позволяет изменять контекст `this` внутри функции и использовать ее с различными объектами.

`const obj = {  
	`name: 'My Object',   
	`printName: function() {   
		`  console.log(this.name);   }, }; 
		` obj.printName.call({ name: 'Another Object' }); // Output: "Another Object"`

`call()` принимает в качестве первого аргумента контекст `this`, а затем последовательно передает аргументы в функцию.

`function sum(a, b) {   return a + b; } console.log(sum.call(null, 1, 2)) // Output: 3`

В случае если контекст не имеет значения, он может быть указан как `null` или `undefined`.

Отличие от `apply()` в том что `call()` принимает аргументы по отдельности, в то время как `apply()` принимает массив аргументов.

[[context]]