# hw-functions

## Темы на повторения 

[Деструктурирующее присваивание](https://learn.javascript.ru/destructuring-assignment)

[Остаточные параметры и оператор расширения](https://learn.javascript.ru/rest-parameters-spread-operator)

[Методы объекта, "this"](https://learn.javascript.ru/object-methods)

### Задача 1
Напишите объект `calculator`.

```
let calculator = {
    init(initialValue = 0) {
        // Ваш код
    },
    addAll(...numbers) {
        // Ваш код
    },
    add(n) {
        // Ваш код
    },
    sub(n) {
        // Ваш код
    },
    mul(n) {
         // Ваш код
    },
    read() {
        // Ваш код
    },
}
```
Примеры для проверки кода

```
calculator.init(1).addAll(1,2,3).read(); // 7
calculator.init().addAll(1,2,3).sub(4).mul(2).read(); // 4
calculator.init(5).add(5).sub(10).read(); // 0
```

### Задача 2
Напишите свой `reduce2`который должен работать аналогично стандартному. 

```
Array.prototype.reduce2 = function(cb, initialValue) {
  // Ваш код
}
```
Примеры для проверки кода


Пример 1
```
[1,2,3,4].reduce2((acc, curr) => {
        acc.push(curr*2);
        return acc;
    }, [1]) 

Output
[1,2,4,6,8]
```
Пример 2
```
[1,2,3,4].reduce2((acc, curr) => acc+=curr)

Output
10
```

Пример 3
```
[1,2,3,4].reduce2((acc, curr) => acc+=curr, 1)

Output
11
```
