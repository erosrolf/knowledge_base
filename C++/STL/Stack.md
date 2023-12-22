***
Один из контейнеров [STL](STL.md)
>для подключения: `#include <stack>`.

> template <class и typedef> одно и то же
```c++
template <class Type, class Container= deque <Type>>
class stack
```
**`Type`** - тип данных элемента для сохранения в стеке.
**`Container`**  - тип базового контейнера, используемый для реализации стека. Значение container по умолчанию — это класс `deque<Type>`.

Подходящие базовые классы контейнеров для стека включают:
[[deque]], [[list]], [[vector]]