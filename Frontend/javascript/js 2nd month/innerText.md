`innerText` - это свойство JavaScript, которое используется для получения или установки текстового содержимого элемента HTML, игнорируя вложенные теги HTML.

Когда вы получаете значение `innerText`, вы получаете строку, содержащую текст внутри элемента, игнорируя вложенные теги. Например:

`let element = document.getElementById("myId"); console.log(element.innerText); // Output: "Hello world"`

Когда вы устанавливаете значение `innerText`, вы заменяете текстовое содержимое элемента с новым текстом. Например:


`let element = document.getElementById("myId"); element.innerText = "Hello world";`

Это свойство работает аналогично свойству `innerHTML`, за исключением того, что оно игнорирует вложенные теги HTML и возвращает только текстовое содержимое.

Например: на html
`<button class='button'>red</button>
`<button class='button'>blue</button>
`<button class='button'>yellow</button>
`<button class='button'>black</button>
`<button class='button'>aqua</button>
`<button class='button'>brown</button>

на javascript пишем следущее:
`const buttons = document.querySelectorAll(.'button')
`for (let button of buttons) {
	`button.addEventListener('click', e => {
		`document.body.style.backroundColor = e.target.innerText})
`}
и когда мы нажимем на каждую кнопку задний фон меняет свой свет это все блогодаря к innerText, innerText принимает с html все style в строку если мы вместо слава блу напишем синий или ещё чтот-то как этот fxcghj то тогда наш код тупо не сработает потому что наш жаваскрипт с html принимает только строку, и здесь меняется свет заднего фона.
[[event]]
