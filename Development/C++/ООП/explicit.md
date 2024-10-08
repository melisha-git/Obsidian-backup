---
tags:
  - oop
---

[[Конструкторы]], получающий единственный [[Аргументы функции|аргумент]], определяют операцию неявного преобразования.

```cpp
complex z1 = 3.14;
complex z2 = z1 * 2;
```

Такое неявное [[Преобразования|преобразования]] не всегда оказывается идеальным. Что бы избежать проблему неявного [[Преобразования|преобразования]] некоторых типов, мы можем определить [[Конструкторы]] следующим образом:

```cpp
class Vector {
public:
	explicit Vector(int s);
};
```

> [!tip]
> - Используйте `explicit` для [[Конструкторы|конструкторов]], который принимает один [[Аргументы функции|аргумент]], если нет всякой причины поступать иначе.

[[!Язык программирования C++. Краткий курс|Источник]]
