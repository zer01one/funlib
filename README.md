# funchero.js
Библиотека для написания функционального кода

## Documentation

### curry

Возвращает обертку для заданной функции. Обёрнутая функция принимает переменное количество аргументов и возвращает новую функцию, которая принимает оставшиеся аргументы, пока функция не будет полностью применена.

**Параметры:**

- `func` - функция, которую нужно обернуть.

**Возвращает:**

- обёрнутая функция.
---

### compose

Возвращает функцию, которая компонует несколько функций в одну функцию.

**Параметры:**

- `funcs` - функции, которые нужно компоновать.

**Возвращает:**

- функция, которая компонует заданные функции.
---

### identify

Возвращает функцию, которая принимает функцию и возвращает новую функцию, которая применяет заданную функцию и возвращает параметр.

**Параметры:**

- `func` - функция, которую нужно применить.

**Возвращает:**

- новая функция, которая применяет заданную функцию и возвращает параметр.
---

### tap

Возвращает функцию, которая принимает функцию и возвращает новую функцию, которая применяет заданную функцию и возвращает параметр.

**Параметры:**

- `func` - функция, которую нужно применить.

**Возвращает:**

- новая функция, которая применяет заданную функцию и возвращает параметр.
---

### alt

Возвращает функцию, которая принимает несколько функций и применяет каждую из них к параметру, пока одна из функций не вернёт истинное значение.

**Параметры:**

- `funcs` - функции, которые нужно применить.

**Возвращает:**

- первая функция, которая вернула истинное значение при применении к параметру.
---

### promising

Возвращает функцию, которая принимает функцию и возвращает новую функцию, которая возвращает промис после применения заданной функции к параметру.

**Параметры:**

- `func` - функция, которую нужно применить.

**Возвращает:**

- новая функция, которая возвращает промис.
---
### fork

Возвращает функцию, которая принимает функцию соединения и несколько функций и возвращает новую функцию, которая применяет заданные функции к параметру и возвращает результат применения функции соединения к результатам применения функций.