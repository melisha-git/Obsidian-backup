---
tags:
  - oop
  - stl
---

Методика получения ресурса в [[Конструкторы|конструкторе]] и освобождение их в [[Деструкторы|деструкторе]] известна, как идиома ***Захват ресурсов есть инициализация*** (Resource Acquisition Is Initialization - RAII) 

RAII позволяет избежать операций с *голым new* - избежать выделения памяти в общем коде. Аналогично, следует избегать голых операций *delete*.

> [!tip]
> - Если [[Конструкторы|конструктор]] (И другие методы [[Классы|класса]]) захватывает ресурс, необходим [[Деструкторы|деструктор]], освобождающий это ресурс

[[!Язык программирования C++. Краткий курс|Источник]]
