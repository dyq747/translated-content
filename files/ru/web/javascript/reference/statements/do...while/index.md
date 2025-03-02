---
title: do...while
slug: Web/JavaScript/Reference/Statements/do...while
---

{{jsSidebar("Statements")}}

Выражение **`do...while`** создаёт цикл, который выполняет указанное выражение до тех пор, пока условие не станет ложным. Условие проверяется после выполнения выражения, то есть выражение выполнится как минимум один раз.

{{InteractiveExample("JavaScript Demo: Statement - Do...While")}}

```js interactive-example
let result = "";
let i = 0;

do {
  i = i + 1;
  result = result + i;
} while (i < 5);

console.log(result);
// Expected output: "12345"
```

## Синтаксис

```
do
   выражение
while (условие);
```

- `выражение`
  - : Выражение, которое выполняется как минимум один раз и выполняется на каждом шаге цикла, пока условие истинно. Выражение может содержать несколько строк, для этого необходимо сгруппировать код в {{jsxref("Statements/block", "блок")}} (`{ ... }`).

<!---->

- `условие`
  - : Выражение, которое вычисляется после каждого шага цикла. Если `условие` истинно, то `выражение` выполняется ещё раз. Когда `условие` ложно, выполняется выражение, следующее после `do...while`.

## Примеры

### Использование `do...while`

В примере, цикл `do...while` выполняется до тех пор, пока `i` не перестанет быть меньше 5.

### HTML

```html
<div id="example"></div>
```

### JavaScript

```js
var result = "";
var i = 0;
do {
  i += 1;
  result += i + " ";
} while (i > 0 && i < 5); // Несмотря на то, что i == 0, цикл всё равно продолжится, так как начинается без теста
document.getElementById("example").innerHTML = result;
```

### Результат

{{ EmbedLiveSample('Примеры') }}

## Спецификации

{{Specifications}}

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- {{jsxref("Statements/while", "while")}}
- {{jsxref("Statements/for", "for")}}
