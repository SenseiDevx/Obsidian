В JavaScript метод `test()` используется для проверки, соответствует ли заданная строка регулярному выражению. Он возвращает значение `true`, если строка соответствует шаблону, и `false` в противном случае.

Синтаксис метода `test()` следующий:
`regexp.test(string)`

где `regexp` - это регулярное выражение, которое нужно проверить, а `string` - это строка, которую нужно проверить на соответствие.

Например, следующий код проверяет, начинается ли строка `str` со слова "Hello":

`let str = "Hello, World!"; let regex = /^Hello/; let result = regex.test(str);  console.log(result); // true`

В этом примере, регулярное выражение `/^Hello/` проверяет, начинается ли строка с символов "Hello". Метод `test()` возвращает `true`, потому что строка `str` начинается со слова "Hello". Если бы строка начиналась с другого слова, метод `test()` возвратил бы `false`.
[[регулярные выражения в жаваскрипт]]