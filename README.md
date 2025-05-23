### Вопрос 1  
**Какое значение присваивается переменной `x` после выполнения следующего кода?**

```python
x = 10
y = 20
if x > y or y > x:
    x = 1
else:
    x = 2
```

- 1  
- 2  
- 10  
- 20  

---

### Вопрос 2
**Как создать гистограмму распределения значений в колонке `A` DataFrame с использованием Matplotlib?**

- `plt.hist(df['A'])`  
- `df.plot(type='histogram', column='A')`  
- `df['A'].draw_hist()`  
- Все вышеперечисленные  

---

### Вопрос 3
**Какое значение будет выведено в результате выполнения следующего кода?**

```python
def flatten(nested_list):
    flat_list = []
    for sublist in nested_list:
        for item in sublist:
            flat_list.append(item)
    return flat_list

nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(flatten(nested_list))
```

- `[1, 2, 3, 4, 5, 6, 7, 8, 9]`  
- `[[1, 2, 3], [4, 5, 6], [7, 8, 9]]`  
- `[1, 2, 3, [4, 5, 6], [7, 8, 9]]`  
- Ошибка  

---

### Вопрос 4
**Что произойдёт при выполнении следующего фрагмента кода?**

```python
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    if num % 2 == 0:
        continue
    print(num, end=' ')
```

- `135`  
- `24`  
- `12345`  
- Ничего не будет выведено  

---

### Вопрос 5
**Какое значение будет иметь переменная `x` после выполнения следующего кода?**

```python
x = 10
y = 2
x /= y + 3
```

- 2.0  
- 2.5  
- 5  
- 7  

---

### Вопрос 6
**Что произойдёт при выполнении следующего кода на Python?**

```python
count = 10
while count < 15:
    print("Текущее значение:", count)
    count += 1
```

- Будет выведено пять строк с сообщением «Текущее значение:» и числами от 10 до 14.  
- Цикл не будет выполнен, так как начальное условие не истинно.  
- Произойдёт бесконечный цикл, так как условие цикла всегда истинно.  
- Программа выдаст ошибку, так как условие цикла некорректно.  

---

### Вопрос 7
**Как можно использовать библиотеку `sqlite3` в Python для выполнения запроса к базе данных?**

- ```python
  import sqlite3
  conn = sqlite3.connect('example.db')
  conn.query('SELECT * FROM table')
  ```  
- ```python
  import sqlite3
  conn = sqlite3.connect('example.db')
  conn.execute('SELECT * FROM table')
  ```  
- ```python
  import sqlite3
  db = sqlite3.query('example.db', 'SELECT * FROM table')
  ```  
- ```python
  import sqlite3
  db = sqlite3.connect('example.db')
  db.select('SELECT * FROM table')
  ```  

---

### Вопрос 8
**В Tkinter, как создать кнопку, которая при нажатии вызывает функцию `say_hello`?**

- ```python
  import tkinter as tk

  def say_hello():
      print("Hello")

  root = tk.Tk()
  button = tk.Button(root, text="Greet", command=say_hello)
  button.pack()
  root.mainloop()
  ```  
- ```python
  import tkinter as tk

  def say_hello():
      print("Hello")

  root = tk.Tk()
  button = tk.Button(root, text="Greet", action=say_hello)
  button.pack()
  root.mainloop()
  ```  
- *(два других варианта кода с ошибками — так, как на скриншоте; включены здесь для полноты)*  
  ```python
  import tkinter as tk

  def say_hello():
      print("Hello")

  root = tk.Tk()
  button = tk.Button(root, text="Greet", command=say_hello)
  button.pack()
  root.mainloop()
  ```
  ```python
  import tkinter as tk

  def say_hello():
      print("Hello")

  root = tk.Tk()
  button = tk.Button(root, text="Greet")
  button = s
  ```  

---

### Вопрос 9  
**В SQLite, как можно изменить тип данных столбца `age` в таблице `users` с `INTEGER` на `TEXT`?**

- A. `ALTER TABLE users MODIFY COLUMN age TEXT;`  
- B. `ALTER TABLE users ALTER COLUMN age TYPE TEXT;`  
- C. `ALTER TABLE users CHANGE age age TEXT;`  
- D. SQLite не поддерживает изменение типа данных столбца напрямую.  

---

### Вопрос 10  
**Как в Python использовать библиотеку `unittest` для создания теста, проверяющего, что функция возвращает правильное значение для определённого входа?**

- A.
  ```python
  import unittest

  def my_function(x):
      return x + 1

  class MyTest(unittest.TestCase):
      def test_my_function(self):
          self.assertEqual(my_function(3), 4)
  ```
- B.
  ```python
  import unittest

  def my_function(x):
      return x + 1

  class MyTest(unittest.TestCase):
      def test_my_function(self):
          assert my_function(3) == 4
  ```
- C.
  ```python
  import unittest

  def my_function(x):
      return x + 1

  class MyTest(unittest.TestCase):
      def check_my_function(self):
          self.assertEqual(my_function(3), 5)
  ```

---

### Вопрос 11  
**Как можно обеспечить безопасное преобразование типа в блоке `try/except`?**

Пример в условии:  
```python
try:
    number = int("not a number")
except ValueError:
    number = 0
```

- A. Код выше корректен для обработки исключения при неверном преобразовании типа.  
- B. Необходимо использовать блок `finally` для присвоения значения `number`.  
- C. Исключение `TypeError` должно быть перехвачено, а не `ValueError`.  
- D. Преобразование типов в Python не может вызывать исключения.  

---

### Вопрос 12  
**Каков результат выполнения выражения `math.prod([2**i for i in range(5)])`, если библиотека `math` импортирована и содержит функцию `prod`?**

- A. 960  
- B. 1024  
- C. 384  
- D. Ошибка  

---

### Вопрос 13  
**Как в Python оптимизировать обработку больших массивов данных с минимальным использованием памяти?**

- A. Использование итераторов вместо списков.  
- B. Применение глобальных переменных для хранения данных.  
- C. Использование библиотеки `multiprocessing` для распределения данных по процессам.  
- D. Хранение всех данных в одном большом списке для уменьшения накладных расходов на управление памятью.  

---

### Вопрос 14  
**Какое значение вернёт следующая функция при вызове `multiply(10, 5)`?**

```python
def multiply(x, y):
    return x * y
```

- A. 15  
- B. 50  
- C. 10  
- D. 5  

---

### Вопрос 15  
**Как в Python реализован полиморфизм?**

- A. С помощью механизма перегрузки методов.  
- B. Через динамическую типизацию и позднее связывание.  
- C. Используя ключевые слова `polymorphic` или `override`.  
- D. С помощью декораторов, указывающих на полиморфные методы.  

---

### Вопрос 16  
**В чём суть паттерна Singleton и как его реализовать с помощью `__new__`?**

- A. Гарантировать, что у класса есть только один экземпляр.  
- B. Создавать неограниченное количество экземпляров класса.  
- C. Гарантировать уникальность значений атрибутов во всех экземплярах.  
- D. Позволять наследование от одного класса к нескольким дочерним.  

---

### Вопрос 17  
**Что такое *data descriptor* в контексте Python ООП?**

- A. Класс, который содержит один метод `__get__`.  
- B. Объект, реализующий методы `__get__` и `__set__`.  
- C. Механизм для определения свойств, которые не хранят данные напрямую.  
- D. Структура данных, поддерживающая быстрый доступ к атрибутам.  

---

### Вопрос 18  
**Что такое инкапсуляция в объектно‑ориентированном программировании?**

- A. Процесс объединения методов и данных, которые манипулируют этими данными, в один класс.  
- B. Способность класса генерировать экземпляры с различными состояниями.  
- C. Способность объекта скрывать свои внутренние компоненты от внешнего мира.  
- D. Механизм объединения объектов в иерархию классов для повышения повторного использования кода.  

---

### Вопрос 19  
**Каков результат выполнения выражения `math.sqrt(16) + pow(2, 3)` при условии, что библиотека `math` импортирована?**

- A. 12.0  
- B. 10.0  
- C. 8.0  
- D. Ошибка  

---

### Вопрос 20  
**В Python, какое исключение будет возбуждено, если пользователь введёт нечисловое значение при попытке преобразования ввода в целое число с помощью функции `int()`?**

- A. `ValueError`  
- B. `TypeError`  
- C. `InputError`  
- D. `SyntaxError`  

---

### Вопрос 21  
**Как отфильтровать строки `DataFrame` в Pandas, где значение в колонке `A` больше 10?**

- A. `df[df['A'] > 10]`  
- B. `df.filter('A > 10')`  
- C. `df.query('A in 10')`  
- D. `df.loc[df['A'] > 10]`  

---

### Вопрос 22  
**Как определить, является ли класс потомком другого класса в Python?**

- A. Использовать функцию `isinstance()`.  
- B. Использовать функцию `issubclass()`.  
- C. Проверить наличие наследуемого класса в списке `__bases__`.  
- D. Использовать оператор `is`.  

---

### Вопрос 23  
**Как в Tkinter привязать событие нажатия клавиши к функции обработки?**

- A. `root.bind('<KeyPress>', handle_keypress)`  
- B. `root.on_key_press('<KeyPress>', handle_keypress)`  
- C. `root.keypress('<KeyPress>', handle_keypress)`  
- D. `root.set_event('<KeyPress>', handle_keypress)`  

---

### Вопрос 24  
**Каков результат выполнения выражения `(lambda x, y: x + y)(3, 4) + (lambda x: x ** 2)(5)`?**

- A. 32  
- B. 47  
- C. 27  
- D. Ошибка  

---

### Вопрос 25  
**Что будет результатом выражения `7 // -3` в Python?**

- A. -2  
- B. -3  
- C. 2  
- D. 3  

---

### Вопрос 26  
**Какой из следующих способов правильно описывает создание защищённого атрибута (*protected*) в классе Python?**

- A. Префикс `_` перед именем атрибута: `_attribute`  
- B. Префикс `__` перед именем атрибута: `__attribute`  
- C. Префикс `protected` перед именем атрибута: `protected attribute`  
- D. Использование декоратора `@protected` перед атрибутом  

---

### Вопрос 27  
**Как проверить, содержится ли ключ `'key1'` в следующем словаре? `dict = {'key1': 100, 'key2': 200, 'key3': 300}`**

- A. `'key1' in dict.keys()`  
- B. `'key1' in dict`  
- C. `dict.contains('key1')`  
- D. `dict.has_key('key1')`  

---

### Вопрос 28  
**Что делает универсальная функция в NumPy?**

- A. Оптимизирует использование памяти  
- B. Применяет операцию ко всем элементам массива  
- C. Объединяет массивы  
- D. Создаёт новые массивы  

---

### Вопрос 29  
**Какой метод используется для сортировки `DataFrame` по значениям одного или нескольких столбцов?**

- A. `align_values()`  
- B. `sort_values()`  
- C. `set_order()`  
- D. Все вышеперечисленные  

---

### Вопрос 30  
**Как в Python оптимизировать обработку больших массивов данных с минимальным использованием памяти?**

- A. Использование итераторов вместо списков.  
- B. Применение глобальных переменных для хранения данных.  
- C. Использование библиотеки `multiprocessing` для распределения данных по процессам.  
- D. Хранение всех данных в одном большом списке для уменьшения накладных расходов на управление памятью.  

--- 

### Вопрос 31 

Как в Python создать кортеж, содержащий только один элемент 50?

**Варианты ответа:**

- `tuple = (50)`
- `tuple = (50,)`
- `tuple = tuple(50)`
- `tuple = [50]`

---


### Вопрос 32 

Предположим, вы используете NumPy для обработки массива данных о температурах за неделю: `temperatures = [22, 25, 19, 21, 23, 24, 20]`. Вы хотите добавить в этот массив значение температуры за следующий день (18 градусов) и рассчитать новую среднюю температуру. Какие действия и команды NumPy вы должны использовать для выполнения этой задачи?

**Варианты ответа:**

- ```python
  temps = np.array(temperatures)
  temps = np.append(temps, 18)
  np.mean(temps)
  ```

- ```python
  temps = np.array(temperatures)
  temps += [18]
  np.average(temps)
  ```

- ```python
  temps = np.array(temperatures)
  temps.append(18)
  np.median(temps)
  ```

- ```python
  temps = np.array(temperatures)
  np.concatenate([temps, [18]])
  np.mean(temps)
  ```

---

### Вопрос 33 

Какой результат даст следующий фрагмент кода?
```python
print("Python", "is", "awesome", sep="-")
```

**Варианты ответа:**

- `Python-is-awesome`
- `Python is awesome`
- `Pythonisawesome`
- `Python - is - awesome`

---

### Вопрос 34 

Каков результат выполнения выражения `math.prod([2**i for i in range(5)])` при условии, что библиотека `math` импортирована и содержит функцию `prod`?

**Варианты ответа:**

- `960`  
- `1024`  
- `384`  
- `Ошибка`

---

### Вопрос 35 

Каким будет результат выполнения следующего кода?

```python
for i in 'hello':
    if i == 'o':
        break
    print(i, end='')
else:
    print(' Done!')
```

**Варианты ответа:**

- `hell`  
- `hello`  
- `hell Done!`  
- `hello Done!`

---


### Вопрос 36 

Что такое data descriptor в контексте Python ООП?

**Варианты ответа:**

- Класс, который содержит один метод `__get__`
- Объект, реализующий методы `__get__` и `__set__`
- Механизм для определения свойств, которые не хранят данные напрямую
- Структура данных, поддерживающая быстрый доступ к атрибутам

---

### Вопрос 37 

Как объявить функцию в Python, которая принимает один параметр?

**Варианты ответа:**

- `def function(p):`
- `def function():`
- `function(p):`
- `def function with p:`

---

### Вопрос 38 

Какой блок позволяет выполнить код независимо от того, произошло исключение или нет?

**Варианты ответа:**

- `try`
- `except`
- `else`
- `finally`

---

### Вопрос 39 

Каков результат выполнения выражения `(lambda x, y: x * y) (3, 4) + (lambda x: x**2) (5)`?

**Варианты ответа:**

- 32
- 47
- 27
- Ошибка

---

### Вопрос 40 

Как можно отсортировать список чисел `nums` по убыванию?

**Варианты ответа:**

- `nums.sort(reverse=True)`
- `sorted(nums, reverse=False)`
- `nums.sorted()`
- `sorted(nums, reverse=True)`

---


### Вопрос 41 

Какое значение присваивается переменной `x` после выполнения следующего кода?

```python
x = 10
y = 20
if x > y or y > x:
    x = 1
else:
    x = 2
```

**Варианты ответа:**

- 1
- 2
- 10
- 20

---

### Вопрос 42 

Какой командой можно отправить изменения из локального репозитория на удалённый репозиторий GitHub?

**Варианты ответа:**

- `git upload`
- `git send`
- `git push`
- `git transfer`

---


### Вопрос 43 

Каков будет результат чтения файла с использованием следующего кода, если файл `example.txt` содержит только строку "Hello Python"?

```python
with open('example.txt', 'r') as file:
    data = file.readline()
    print(data)
```

**Варианты ответа:**

- Выведет 'Hello Python'
- Выведет 'Hello Python\n'
- Выведет ['Hello Python']
- Возникнет ошибка

---

### Вопрос 44 

Как получить 25-й и 75-й перцентили колонки DataFrame в Pandas?

**Варианты ответа:**

- Использовать функцию `get_percentiles([0.25, 0.75])`
- Использовать метод `quantile([0.25, 0.75])`
- Применить `percentiles([25, 75])`
- Вызвать `describe([0.25, 0.75])` и извлечь нужные значения

---

### Вопрос 45 

Что делает файл `__init__.py` в структуре модуля Python?

**Варианты ответа:**

- Позволяет использовать модуль как библиотеку в C++
- Обеспечивает совместимость с Jupyter
- Позволяет интерпретатору Python распознавать директорию как пакет
- Создает виртуальное окружение

---

### Вопрос 46 

Каков результат выполнения следующего фрагмента кода?

```python
a = 5
b = 2
print(a // b)
```

**Варианты ответа:**

- 2
- 2.5
- Ошибка времени выполнения
- 3

---

### Вопрос 47

Какой из следующих кодов корректно объединит список строк `['Python', 'is', 'awesome']` в одну строку, используя пробел в качестве разделителя?

**Варианты ответа:**

- `""join(['Python', 'is', 'awesome'])`
- `""join(['Python', 'is', 'awesome'])`
- `join('', ['Python', 'is', 'awesome'])`
- `''.join(['Python', 'is', 'awesome'])`

---

### Вопрос 48

Как использовать Python для асинхронного получения данных из нескольких API?

**Варианты ответа:**

- Использование библиотеки `requests` в цикле `for`.
- Применение асинхронных запросов с `asyncio` и `aiohttp`.
- Запуск множества потоков, каждый из которых делает синхронный HTTP запрос.
- Использование одновременных вызовов `subprocess.Popen` для каждого API.

---

### Вопрос 49

Какой объект в Matplotlib используется для создания графика?

**Варианты ответа:**

- `Figure`
- `Canvas`
- `Plotter`
- `Drawer`

---

### Вопрос 50

Какой из следующих способов правильно описывает создание защищенного атрибута (protected) в классе Python?

**Варианты ответа:**

- Префикс перед именем атрибута: `_attribute`
- Префикс - перед именем атрибута: `_attribute`
- Префикс `protected` перед именем атрибута: `protected attribute`
- Использование декоратора `@protected` перед атрибутом

---

### Вопрос 51

Каким образом можно обеспечить, чтобы функция `print()` не добавляла символ новой строки в конце вывода, и вместо этого добавляла тире (-)?

**Варианты ответа:**

- Использовать параметр `end='-'`
- Использовать параметр `sep='-'`
- Использовать параметр `stop='-'`
- Использовать параметр `finish='-'`

---

### Вопрос 52

Как преобразовать длинный формат данных DataFrame в широкий формат?

**Варианты ответа:**

- Использовать `pivot()`
- Применить `transform_to_wide()`
- Вызвать `spread()`
- Использовать `reshape_to_wide()`

---

### Вопрос 53

Что позволяет вычислить функция `corr()` в Pandas?

**Варианты ответа:**

- Дисперсию значений в столбце
- Корреляцию между столбцами в DataFrame
- Стандартное отклонение набора данных
- Все вышеперечисленные

---

### Вопрос 54 

Каков результат операции сложения векторов `[1, 2, 3]` и `[4, 5, 6]`?

**Варианты ответа:**

- `[5, 7, 9]`
- `[1, 2, 3, 4, 5, 6]`
- `[4, 6, 8]`
- Ошибка

---

### Вопрос 55

Как преобразовать все строки в колонке DataFrame в Pandas к нижнему регистру?

**Варианты ответа:**

- `df['column'].str.lower()`
- `df['column'].to_lower()`
- `df.lowercase('column')`
- `df['column'].apply(str.lower)`

---

### Вопрос 56

Как создать копию словаря в Python, чтобы изменения в копии не отражались на оригинале?

**Варианты ответа:**

- `new_dict = dict(old_dict)`
- `new_dict = old_dict.copy()`
- `new_dict = copy(old_dict)`
- `new_dict = old_dict`

---
