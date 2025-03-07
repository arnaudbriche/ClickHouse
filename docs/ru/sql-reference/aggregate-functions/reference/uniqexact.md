---
slug: /ru/sql-reference/aggregate-functions/reference/uniqexact
sidebar_position: 191
---

# uniqExact {#agg_function-uniqexact}

Вычисляет точное количество различных значений аргументов.

``` sql
uniqExact(x[, ...])
```

Функцию `uniqExact` следует использовать, если вам обязательно нужен точный результат. В противном случае используйте функцию [uniq](/ru/sql-reference/aggregate-functions/reference/uniq).

Функция `uniqExact` расходует больше оперативной памяти, чем функция `uniq`, так как размер состояния неограниченно растёт по мере роста количества различных значений.

**Аргументы**

Функция принимает переменное число входных параметров. Параметры могут быть числовых типов, а также `Tuple`, `Array`, `Date`, `DateTime`, `String`.

**Смотрите также**

-   [uniq](/ru/sql-reference/aggregate-functions/reference/uniq.md#agg_function-uniq)
-   [uniqCombined](/ru/sql-reference/aggregate-functions/reference/uniq.md#agg_function-uniqcombined)
-   [uniqHLL12](/ru/sql-reference/aggregate-functions/reference/uniq.md#agg_function-uniqhll12)
