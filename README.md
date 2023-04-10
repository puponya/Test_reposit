# Test_reposit
# Параграф
---
  Параграф — это одна или несколько подряд идущих строчек текста, отделённых одной или несколькими пустыми строчками. Если строка содержит только пробелы или табы, то она всё равно считается пустой.<br>Подряд идущие строчки будут склеены в одну, если не добавить жёсткий перенос. Существует несколько способов, как это можно сделать.
## Многоуровневый список
- Уровень списка 1. Пункт 1.
    - Уровень списка 2. Пункт 1.
- Уровень списка 1. Пункт 2.
    - Уровень списка 2. Пункт 1.
    - Уровень списка 2. Пункт 2.
- Уровень списка 1. Пункт 3.
    - Уровень списка 2. Пункт 1.
        - Уровень списка 3. Пункт 1.
        - Уровень списка 3. Пункт 2.
           - Уровень списка 4. Пункт 1.
---
# Статистика
---
В README-файл профиля можно добавлять различные виджеты со статистическими данными о себе и свой деятельности на GitHub. Данные автоматически обновляются с некоторой периодичностью и в профиле всегда отображается актуальная информация.
---
### Блок кода
```
from timeit import Timer

tmp = "Python 3.2.2 (default, Jun 12 2011, 15:08:59) [MSC v.1500 32 bit (Intel)] on win32."

def case1(): # А. инкрементальные конкатенации в цикле
    s = ""
    for i in range(10000):
        s += tmp

def case2(): # Б. через промежуточный список и метод join
    s = []
    for i in range(10000):
        s.append(tmp)
    s = "".join(s)

def case3(): # В. списковое выражение и метод join
    return "".join([tmp for i in range(10000)])

def case4(): # Г. генераторное выражение и метод join
    return "".join(tmp for i in range(10000))

for v in range(1,5):
    print (Timer("func()","from __main__ import case%s as func" % v).timeit(200))
```
### Цитаты
> Цитата (уровень 11)    
> > Вложенная цитата (уровень 22)    
> > > Вложенная цитата (уровень 33)
# Картинка
![Картинка](https://klike.net/uploads/posts/2019-05/1556708032_1.jpg)
# For more info
For more information, see the [calculator file](calculator.md).
# Добавьте больше картинок
