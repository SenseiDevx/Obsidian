"Super" в JavaScript это ключевое слово, которое используется внутри классов и методов для обращения к родительскому классу или методу.

-   Если "super" используется внутри конструктора класса, то он вызывает родительский конструктор. Это необходимо для инициализации свойств родительского класса перед инициализацией свойств дочернего класса.
-   Если "super" используется внутри метода, то он вызывает родительский метод с теми же аргументами. Это может быть использовано для добавления новой функциональности к существующему методу или для изменения его поведения.

Например:

javascriptCopy code

`class Parent {   constructor(name) {     this.name = name;   }   sayName() {     console.log(this.name);   } }  class Child extends Parent {   constructor(name, age) {     super(name);     this.age = age;   }   sayAge() {     console.log(this.age);   }   sayNameAndAge() {     super.sayName();     this.sayAge();   } }`
[[class в js]]