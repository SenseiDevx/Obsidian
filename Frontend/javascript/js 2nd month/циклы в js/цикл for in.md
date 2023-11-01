`for in` чаще всего применяется к объектам (object)

`for-in` цикл в JavaScript - это конструкция, которая позволяет перебрать свойства объекта. Он используется в том случае, когда вы хотите перебрать не сами элементы объекта, а их ключи (имена свойств).

Синтаксис `for-in` цикла выглядит следующим образом:

`for (variable in object) {   // code to be executed }`

-   `variable` - это переменная, которая будет присваиваться каждому ключу объекта в ходе итерации.
-   `object` - это объект, свойства которого нужно перебрать.

const person = {
name: 'John', 
age: 30, 
job: 'developer' 
}; 
for (const key in person) { console.log(`Ключ:${key},Значение: ${person[key]}`); }
В этом коде мы создаем объект `person` с тремя свойствами: `name`, `age`, `job`. Затем мы используем `for-in` цикл для перебора свойств этого объекта. На каждой итерации цикла переменная `key` будет присваиваться названию текущего свойства, а значение свойства будет выведено в консоль. Результатом выполнения этого кода будет вывод в консоль следующего:


`Ключ: name, Значение: John 
`Ключ: age, Значение: 30
`Ключ: job, Значение: developer`

`let obj = {  
`    string: 'some str',  
`    number: 42,  
`    'key': false,  
 ``   [null]: {  
   `     name: 'Nurdin'  
    `},  
    `sayHi() {  
      `  console.log('HI')  
    `}  
`}  
  
`console.log(obj["key"])  
`console.log(obj["number"])  
`console.log(obj["string"])  
`console.log(obj[null])  
  
`obj.sayHi()  
`console.log(obj.sayHi())
`for (let key in obj) {  
`    console.log(`Ключ:${key},Значение: ${obj[key]}`)  
`}
в консоль выведет:
`Ключ: string, Значение: some str
`Ключ: number, Значение: 42
`Ключ: key, Значение: false
`Ключ: null, Значение: [object Object]
`Ключ: sayHi, Значение: sayHi() {
`         console.log('HI')
`     }

[[циклы в jc]]