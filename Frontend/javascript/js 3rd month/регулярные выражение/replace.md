В JavaScript метод `replace()` используется для замены текста в строке с использованием регулярных выражений. Он возвращает новую строку, в которой заменены все совпадения с заданным шаблоном.

Синтаксис метода `replace()` следующий:

`string.replace(regexp|substr, newSubStr|function)`

где `string` - это строка, в которой необходимо выполнить замену, `regexp` - это регулярное выражение, которое определяет шаблон поиска, `substr` - это строка, которую необходимо заменить, `newSubStr` - это новая строка, на которую будет производиться замена, `function` - это функция, которая будет вызываться для каждого совпадения и возвращать новую строку замены.

Например, следующий код заменяет все совпадения со словом "Hello" в строке `str` на слово "Hi":

`let str = "Hello, World! Hello, JavaScript!"; let regex = /Hello/g; let result = str.replace(regex, "Hi");  console.log(result); // "Hi, World! Hi, JavaScript!"`

В этом примере, регулярное выражение `/Hello/g` ищет все вхождения слова "Hello" в строке `str`. Метод `replace()` заменяет все найденные совпадения на слово "Hi", возвращая новую строку "Hi, World! Hi, JavaScript!".
[[регулярные выражения в жаваскрипт]]