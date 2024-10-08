---
tags:
  - oop
---

в C++ имеется конструкция `= delete`, указывающая, что данная операция не должна генерироваться.

Например:

```cpp
class Y {
public:
	Y() = delete; // Не генерировать конструктор по умолчанию
	Y(const Y&) = delete; // Не генерировать конструктор копирования
	Y(Y&&) = default; // По умолчанию конструктор перемещения
};
```

Конструкция `= delete` приводит к тому, что попытка использования [[Функции|функции]] является ошибкой времени компиляции и может быть использована для любых [[Функции|функций]].

[[!Язык программирования C++. Краткий курс|Источник]]
