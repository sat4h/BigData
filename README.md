# BigData

## Ионов Артем группа 6131-010402D

### [1. Лабораторная работа](https://github.com/sat4h/BigData/blob/7380e521c8fa54dd27f0a04f02de5cdb855d0114/LR1/BigDataIonovLR1.ipynb)

### [2. Лабораторная работа](https://github.com/sat4h/BigData/tree/7380e521c8fa54dd27f0a04f02de5cdb855d0114/LR2)

### [3. Лабораторная работа](https://github.com/sat4h/BigData/tree/e851b150374a6c558a3ab270f033f95807d36756/LR3)

### [4. Лабораторная работа](https://github.com/sat4h/BigData/tree/980b97ea7e2454cfc6757875033cd6b7c6351b05/LR4)

**Вопросы по Spark:**

**1. Каким образом можно удалить первый и последний столбец таблицы в Spark? два варианта**

Есть два варианта:
1. использовать метод select, перечислив столбцы, которые нужно оставить:
df = df.select(*df.columns[1:-1])

2. Использовать метод drop, удаляя столбцы по имени:
df = df.drop(df.columns[0]).drop(df.columns[-1])

**2. Могут ли возникнуть проблемы если начать обработку RDD в котором 80% записей принадлежит одному ключу?**
