Array.prototype.filter() - это метод JavaScript, который создает новый массив со всеми элементами, для которых предоставленная функция callback возвращает true. Этот метод используется для фильтрации элементов массива по определенному условию. Например:


`const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]; 
`const evenNumbers = numbers.filter(number => number % 2 === 0); 
`console.log(evenNumbers); // [2, 4, 6, 8, 10]`

В этом примере мы использовали метод filter для получения массива с четными числами из исходного массива numbers.

мой пример: 

`const fruits = ['apple', 'pineapple', 'peach', 'grape'`]
`console.log(fruits)
`const result = fruits.filter(fruit => {
	`return fruit.length > 5`
``})

`console.log(result)`

то нам уже в консоль выведет следующее значение: 
0: "apple"
1: "pineapple"
2: "peach"
3: "grape"``
length: 4 (это первый массив)
а во втором массиве будет только pineapple потому что этот фильтр отфильтровывал и вывел нам в консоль только те слово которое буквы больше 5 знаков.

[[методы массивов в jc]]