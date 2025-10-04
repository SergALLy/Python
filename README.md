[python_course_les1.ipynb](https://github.com/user-attachments/files/22699831/python_course_les1.ipynb)
{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Введение в программирование на Python\n",
    "\n",
    "Добро пожаловать на первый урок по программированию на Python! Сегодня мы познакомимся с основными понятиями, которые помогут вам начать писать простые программы. Не переживайте, если вы никогда раньше не программировали — мы всё объясним подробно и простыми словами.\n",
    "\n",
    "## Что такое Python?\n",
    "\n",
    "Python — это язык программирования, который позволяет людям общаться с компьютером с помощью специального кода. Этот код похож на инструкции, которые мы даём компьютеру, чтобы он выполнил определённые действия.\n",
    "\n",
    "---\n",
    "\n",
    "# 1. Типы данных в Python и преобразование типов данных\n",
    "\n",
    "В программировании данные могут быть разных типов. Представьте, что тип данных — это как категория или вид информации, с которой вы работаете.\n",
    "\n",
    "## Основные типы данных:\n",
    "\n",
    "1. **Числа (Numbers)**:\n",
    "   - **Целые числа (int)**: это числа без дробной части, например, 1, 42, -5.\n",
    "   - **Вещественные числа (float)**: это числа с дробной частью, например, 3.14, -0.001, 2.0.\n",
    "   - **Комплексные числа (complex)**: числа с действительной и мнимой частью, например, `1 + 2j`.\n",
    "\n",
    "2. **Строки (str)**:\n",
    "   - Это последовательность символов, например, слова или предложения: \"Привет\", \"Python\", \"123\".\n",
    "\n",
    "3. **Логические значения (bool)**:\n",
    "   - Имеют только два значения: `True` (истина) или `False` (ложь).\n",
    "\n",
    "4. **NoneType**:\n",
    "   - Представляет отсутствие значения. Единственное значение этого типа — `None`.\n",
    "\n",
    "---\n",
    "\n",
    "## Примеры:\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "# Целое число\n",
    "age = 15\n",
    "\n",
    "# Вещественное число\n",
    "temperature = 36.6\n",
    "\n",
    "# Комплексное число\n",
    "z = 2 + 3j\n",
    "\n",
    "# Строка\n",
    "greeting = \"Здравствуйте\"\n",
    "\n",
    "# Логическое значение\n",
    "is_student = True\n",
    "\n",
    "# Отсутствие значения\n",
    "result = None"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Проверка типа данных\n",
    "\n",
    "Вы можете проверить тип данных переменной с помощью функции `type()`:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(type(age))        # <class 'int'>\n",
    "print(type(temperature))  # <class 'float'>\n",
    "print(type(greeting))     # <class 'str'>\n",
    "print(type(is_student))   # <class 'bool'>\n",
    "print(type(result))       # <class 'NoneType'>"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Преобразование типов данных\n",
    "\n",
    "Иногда нам нужно изменить тип данных, чтобы выполнить определённые операции.\n",
    "\n",
    "### Почему это важно?\n",
    "\n",
    "- Вы не можете складывать число и строку напрямую.\n",
    "- Преобразование позволяет избежать ошибок и выполнять нужные операции.\n",
    "\n",
    "### Основные функции для преобразования:\n",
    "\n",
    "- `int()` — преобразует значение в целое число.\n",
    "- `float()` — преобразует значение в вещественное число.\n",
    "- `str()` — преобразует значение в строку.\n",
    "- `bool()` — преобразует значение в логическое.\n",
    "\n",
    "---\n",
    "\n",
    "## Примеры преобразования:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "# Преобразование строки в число\n",
    "number_str = \"42\"\n",
    "number_int = int(number_str)  # Теперь это число 42\n",
    "\n",
    "# Преобразование строки с дробной частью\n",
    "float_str = \"3.14\"\n",
    "number_float = float(float_str)  # Теперь это число 3.14\n",
    "\n",
    "# Преобразование числа в строку\n",
    "age = 15\n",
    "age_str = str(age)  # Теперь это строка \"15\"\n",
    "\n",
    "# Преобразование числа в логическое значение\n",
    "zero = 0\n",
    "print(bool(zero))  # Выведет: False\n",
    "\n",
    "non_zero = 5\n",
    "print(bool(non_zero))  # Выведет: True"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " 2. Операции над переменными\n",
    "\n",
    "Переменные — это контейнеры для хранения данных.\n",
    "\n",
    "## Присваивание переменных"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "x = 10  # Теперь переменная x содержит число 10\n",
    "name = \"Алиса\"  # Переменная name содержит строку \"Алиса\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Правила именования переменных:\n",
    "\n",
    "- Имена переменных должны начинаться с буквы или символа подчёркивания `_`.\n",
    "- Можно использовать буквы, цифры и символы подчёркивания.\n",
    "- Имена чувствительны к регистру: `age` и `Age` — разные переменные.\n",
    "- Не используйте зарезервированные слова (например, `if`, `while`, `class`).\n",
    "\n",
    "---\n",
    "\n",
    "## Арифметические операции\n",
    "\n",
    "Вы можете выполнять математические операции с числами.\n",
    "\n",
    "- **Сложение**: `+`\n",
    "- **Вычитание**: `-`\n",
    "- **Умножение**: `*`\n",
    "- **Деление**: `/` (результат — вещественное число)\n",
    "- **Целочисленное деление**: `//` (результат — целое число)\n",
    "- **Остаток от деления**: `%`\n",
    "- **Возведение в степень**: `**`\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = 5\n",
    "b = 2\n",
    "\n",
    "sum_result = a + b      # Результат: 7\n",
    "diff_result = a - b     # Результат: 3\n",
    "prod_result = a * b     # Результат: 10\n",
    "div_result = a / b      # Результат: 2.5\n",
    "int_div_result = a // b # Результат: 2\n",
    "mod_result = a % b      # Результат: 1\n",
    "power_result = a ** b   # Результат: 25"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Операции со строками\n",
    "\n",
    "- **Конкатенация (соединение)**: `+`\n",
    "- **Повторение строки**: `*`\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "first_name = \"Иван\"\n",
    "last_name = \"Петров\"\n",
    "\n",
    "full_name = first_name + \" \" + last_name  # Результат: \"Иван Петров\"\n",
    "\n",
    "laugh = \"ха\"\n",
    "laugh_three_times = laugh * 3  # Результат: \"хахаха\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Индексация строк:\n",
    "\n",
    "- Обращение к символам по индексу (начиная с 0):"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "word = \"Python\"\n",
    "print(word[0])  # 'P'\n",
    "print(word[2])  # 't'"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Длина строки:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [
    {
     "ename": "",
     "evalue": "",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31mRunning cells with 'Python 3.10.11' requires the ipykernel package.\n",
      "\u001b[1;31mInstall 'ipykernel' into the Python environment. \n",
      "\u001b[1;31mCommand: '\"d:/Visial code/MinGW/ucrt64/bin/python.exe\" -m pip install ipykernel -U --user --force-reinstall'"
     ]
    }
   ],
   "source": [
    "message = \"Привет\"\n",
    "print(len(message))  # Выведет: 6"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Что нельзя делать\n",
    "\n",
    "- Нельзя складывать число и строку без преобразования типов.\n",
    "\n",
    "### Пример ошибки:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "age = 15\n",
    "message = \"Мне \" + age  # Ошибка!\n",
    "\n",
    "# Правильно:\n",
    "message = \"Мне \" + str(age)  # Результат: \"Мне 15\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- Нельзя делить на ноль:\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [
    {
     "ename": "",
     "evalue": "",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31mRunning cells with 'Python 3.10.11' requires the ipykernel package.\n",
      "\u001b[1;31mInstall 'ipykernel' into the Python environment. \n",
      "\u001b[1;31mCommand: '\"d:/Visial code/MinGW/ucrt64/bin/python.exe\" -m pip install ipykernel -U --user --force-reinstall'"
     ]
    }
   ],
   "source": [
    "x = 10\n",
    "y = 0\n",
    "result = x / y  # Ошибка ZeroDivisionError"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# 3. Ввод и вывод данных\n",
    "\n",
    "Чтобы программа могла общаться с пользователем, используются функции `input()` и `print()`.\n",
    "\n",
    "## Функция `print()`\n",
    "\n",
    "Выводит информацию на экран.\n",
    "\n",
    "### Синтаксис:\n",
    "\n",
    "```python\n",
    "print(value, ..., sep=' ', end='\\n')\n",
    "```\n",
    "\n",
    "- **`value`** — значения для вывода.\n",
    "- **`sep`** — разделитель между значениями (по умолчанию пробел).\n",
    "- **`end`** — символ, который добавляется в конце (по умолчанию новая строка).\n",
    "\n",
    "### Пример:\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(\"Привет, мир!\")  # Выведет: Привет, мир!\n",
    "print(\"Python\", \"очень\", \"крутой\", sep=\"-\")  # Выведет: Python-очень-крутой"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Функция `input()`\n",
    "\n",
    "Позволяет пользователю ввести данные с клавиатуры.\n",
    "\n",
    "### Синтаксис:\n",
    "\n",
    "```python\n",
    "variable = input(prompt)\n",
    "```\n",
    "\n",
    "- **`prompt`** — сообщение или подсказка для пользователя.\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "name = input(\"Как тебя зовут? \")\n",
    "print(\"Привет, \" + name + \"!\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**Важно:** `input()` всегда возвращает строку. Если нужно получить число, используйте преобразование типов.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "age = int(input(\"Сколько тебе лет? \"))\n",
    "print(\"Через год тебе будет\", age + 1)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## f-строки (форматированные строки)\n",
    "**f-строки** (от \"formatted strings\") — это способ вставлять значения переменных прямо внутрь строк, используя выражение `{}`. Они появились в Python 3.6 и позволяют делать код более читаемым и компактным.\n",
    "\n",
    "### Синтаксис f-строк\n",
    "\n",
    "Чтобы использовать f-строки, перед открывающей кавычкой строки нужно поставить букву `f` или `F`.\n",
    "\n",
    "### Синтаксис:\n",
    "\n",
    "```python\n",
    "f\"текст {переменная} текст\"\n",
    "```\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "name = \"Алиса\"\n",
    "age = 21\n",
    "\n",
    "message = f\"Меня зовут {name}, мне {age} лет.\"\n",
    "print(message)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Форматирование данных внутри f-строк\n",
    "\n",
    "Вы можете управлять тем, как будут отображаться данные внутри f-строки, используя форматные спецификаторы. Форматирование осуществляется после двоеточия `:` внутри фигурных скобок.\n",
    "\n",
    "#### Общий синтаксис\n",
    "```python\n",
    "f\"{переменная:спецификатор_форматирования}\"\n",
    "```\n",
    "### Форматирование чисел\n",
    "\n",
    "#### 1. Вещественные числа (float)\n",
    "\n",
    "Вы можете задать количество знаков после запятой, используя спецификатор `.nf`, где `n` — число знаков.\n",
    "\n",
    "**Пример:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "pi = 3.14159265\n",
    "print(f\"Число пи приблизительно равно {pi:.2f}\")\n",
    "# Выведет: Число пи приблизительно равно 3.14"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **`.2f`** означает, что число будет отображено с 2 знаками после запятой.\n",
    "- **`.3f`** — с 3 знаками и т.д.\n",
    "\n",
    "#### 2. Целые числа (int)\n",
    "\n",
    "Вы можете задавать минимальную ширину поля для отображения числа, дополнение нулями и выравнивание.\n",
    "\n",
    "**Примеры:**\n",
    "\n",
    "- **Минимальная ширина поля:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "number = 7\n",
    "print(f\"Число: {number:5}\")\n",
    "# Выведет: Число:     7\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " Здесь `5` — ширина поля, число будет выравнено по правому краю.\n",
    "\n",
    "- **Дополнение нулями:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Номер заказа: 042\n"
     ]
    }
   ],
   "source": [
    "number = 42\n",
    "print(f\"Номер заказа: {number:03}\")\n",
    "# Выведет: Номер заказа: 042"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Здесь `0` перед `3` указывает на дополнение нулями до ширины 3 символа.\n",
    "\n",
    "- **Выравнивание:**\n",
    "\n",
    "  - **По правому краю (по умолчанию):**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "|   42|\n"
     ]
    }
   ],
   "source": [
    "print(f\"|{number:>5}|\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " - **По левому краю:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(f\"|{number:<5}|\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " - **По центру:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(f\"|{number:^5}|\")\n",
    "# Выведет: | 42  |"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "#### 3. Отображение чисел в разных системах счисления\n",
    "\n",
    "- **Двоичная система (binary):**\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "number = 255\n",
    "print(f\"Двоичное: {number:b}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **Восьмеричная система (octal):**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(f\"Восьмеричное: {number:o}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **Шестнадцатеричная система (hexadecimal):**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(f\"Шестнадцатеричное: {number:x}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "#### 4. Процентное представление\n",
    "\n",
    "Отображение числа в виде процентов."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "success_rate = 0.85\n",
    "print(f\"Уровень успеха: {success_rate:.0%}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **`.0%`** означает, что число будет умножено на 100 и отображено без десятичных знаков со знаком `%`.\n",
    "\n",
    "---\n",
    "\n",
    "### Форматирование строк\n",
    "\n",
    "#### 1. Обрезка и ограничение длины\n",
    "\n",
    "Вы можете ограничить максимальную длину отображаемой строки.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "text = \"Python — замечательный язык программирования\"\n",
    "print(f\"{text:.10}\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **`.10`** означает, что будет отображено только первые 10 символов строки.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Другие типы строк в Python\n",
    "\n",
    "В Python строки могут иметь специальные префиксы, которые изменяют их поведение.\n",
    "\n",
    "### 1. r-строки (raw strings)\n",
    "\n",
    "#### Что такое r-строки?\n",
    "\n",
    "**r-строки** или **сырые строки** — это строки, в которых символы обратного слеша `\\` не интерпретируются как специальные символы (экранирование), а остаются как есть.\n",
    "\n",
    "#### Зачем нужны r-строки?\n",
    "\n",
    "- Удобны при работе с регулярными выражениями.\n",
    "- Упрощают запись путей к файлам в Windows.\n",
    "- Позволяют избежать ошибок, связанных с некорректным экранированием.\n",
    "\n",
    "#### Синтаксис\n",
    "\n",
    "Перед открывающей кавычкой строки ставится буква `r` или `R`."
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "path = r\"C:\\new_folder\\test.txt\"\n",
    "print(path)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "# Обычная строка\n",
    "path = \"C:\\\\new_folder\\\\test.txt\"\n",
    "print(path)\n",
    "# Выведет: C:\\new_folder\\test.txt\n",
    "\n",
    "# r-строка\n",
    "path = r\"C:\\new_folder\\test.txt\"\n",
    "print(path)\n",
    "# Выведет: C:\\new_folder\\test.txt\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# 4. Коллекции данных\n",
    "\n",
    "Коллекции позволяют хранить несколько значений в одной переменной.\n",
    "\n",
    "## Списки (list)\n",
    "\n",
    "- Изменяемые, упорядоченные коллекции.\n",
    "\n",
    "### Создание списка:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "fruits = [\"яблоко\", \"банан\", \"вишня\"]"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Обращение к элементам:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(fruits[0])  # Выведет: яблоко\n",
    "print(fruits[-1]) # Выведет: вишня (обращение с конца)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Изменение элементов:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "fruits[1] = \"апельсин\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Добавление элемента:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "fruits.append(\"манго\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Удаление элемента:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "fruits.remove(\"яблоко\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Кортежи (tuple)\n",
    "\n",
    "- Неизменяемые, упорядоченные коллекции.\n",
    "\n",
    "### Создание кортежа:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "colors = (\"красный\", \"зелёный\", \"синий\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Обращение к элементам:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(colors[1])  # Выведет: зелёный"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**Важно:** Элементы кортежа изменить нельзя."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Множества (set)\n",
    "\n",
    "- Неупорядоченные коллекции без повторяющихся элементов.\n",
    "\n",
    "### Создание множества:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "numbers = {1, 2, 3, 2, 1}\n",
    "print(numbers)  # Выведет: {1, 2, 3}"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Добавление элемента:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "numbers.add(4)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "\n",
    "## Словари (dict)\n",
    "\n",
    "- Коллекции пар \"ключ-значение\".\n",
    "\n",
    "### Создание словаря:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "student = {\n",
    "    \"name\": \"Иван\",\n",
    "    \"age\": 16,\n",
    "    \"grade\": \"10 класс\"\n",
    "}"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Обращение к значениям:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "print(student[\"name\"])  # Выведет: Иван"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Добавление нового ключа:\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "student[\"city\"] = \"Москва\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# 5. Особенности Python и полезные советы\n",
    "# Комментарии\n",
    "\n",
    "- Используются для пояснений в коде.\n",
    "- Не выполняются программой.\n",
    "\n",
    "### Однострочный комментарий:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "# Это комментарий\n",
    "print(\"Это код\")"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Многострочный комментарий:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "\"\"\"\n",
    "Это\n",
    "многострочный\n",
    "комментарий\n",
    "\"\"\""
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Полезные фишки\n",
    "\n",
    "- **Одновременное присваивание нескольких переменных:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a, b, c = 1, 2, 3"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **Обмен значениями переменных:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a, b = b, a"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- **Генераторы списков:**"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "squares = [x**2 for x in range(1, 6)]\n",
    "print(squares)  # [1, 4, 9, 16, 25]"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " 6. Организация памяти в Python\n",
    "\n",
    "Понимание того, как Python управляет памятью, поможет вам писать более эффективный код и избегать распространённых ошибок.\n",
    "\n",
    "## Переменные и объекты\n",
    "\n",
    "В Python **всё является объектом**. Когда вы создаёте переменную и присваиваете ей значение, вы создаёте объект в памяти, а переменная ссылается на этот объект.\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = 10"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- Здесь `10` — это объект типа `int`, сохранённый в памяти.\n",
    "- Переменная `a` ссылается на этот объект.\n",
    "\n",
    "---\n",
    "\n",
    "## Идентификаторы объектов\n",
    "\n",
    "Каждый объект в памяти имеет уникальный идентификатор, который можно узнать с помощью функции `id()`.\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = 10\n",
    "print(id(a))  # Выведет уникальный идентификатор объекта 10"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Неизменяемые и изменяемые объекты\n",
    "\n",
    "### Неизменяемые объекты (Immutable):\n",
    "\n",
    "- **Примеры**: `int`, `float`, `str`, `tuple`, `bool`\n",
    "- После создания их значение изменить нельзя.\n",
    "\n",
    "### Изменяемые объекты (Mutable):\n",
    "\n",
    "- **Примеры**: `list`, `dict`, `set`\n",
    "- Их содержимое можно изменить после создания.\n",
    "\n",
    "---\n",
    "\n",
    "## Почему это важно?\n",
    "\n",
    "Понимание разницы между изменяемыми и неизменяемыми объектами помогает избежать неожиданных результатов в программе.\n",
    "\n",
    "### Пример с неизменяемым объектом:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a= 5\n",
    "b = a\n",
    "a = a + 1\n",
    "\n",
    "print(a)  # Выведет: 6\n",
    "print(b)  # Выведет: 5"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- `a` и `b` сначала ссылаются на один и тот же объект `5`.\n",
    "- Когда мы делаем `a = a + 1`, создаётся новый объект `6`, и `a` теперь ссылается на него.\n",
    "- `b` продолжает ссылаться на `5`.\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "### Пример с изменяемым объектом:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "list1 = [1, 2, 3]\n",
    "list2 = list1\n",
    "list1.append(4)\n",
    "\n",
    "print(list1)  # Выведет: [1, 2, 3, 4]\n",
    "print(list2)  # Выведет: [1, 2, 3, 4]"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "- `list1` и `list2` ссылаются на один и тот же список.\n",
    "- Изменения через `list1` отразились и на `list2`."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Управление памятью и сборщик мусора\n",
    "\n",
    "Python автоматически управляет памятью с помощью **сборщика мусора** (Garbage Collector).\n",
    "\n",
    "- Когда объект больше не имеет ссылок на него, он считается недостижимым.\n",
    "- Сборщик мусора освобождает память, удаляя такие объекты.\n",
    "\n",
    "### Пример:"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": [
    "a = [1, 2, 3]\n",
    "a = None  # Список [1, 2, 3] больше не имеет ссылок и может быть удалён из памяти"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Практические советы\n",
    "\n",
    "- **Осторожно с изменяемыми объектами**: если несколько переменных ссылаются на один изменяемый объект, изменение через одну переменную отразится на всех остальных.\n",
    "\n",
    "- **Используйте копирование**, если нужно создать независимую копию изменяемого объекта:\n",
    "  - Для поверхностного копирования списков: `new_list = old_list.copy()`\n",
    "  - Для глубокого копирования: `new_list = copy.deepcopy(old_list)`\n",
    "\n",
    "- **Не изменяйте объекты внутри функций**, если не уверены в последствиях."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# Практические задания для закрепления материала\n",
    "\n",
    "Чтобы лучше усвоить изученные темы, выполните следующие задачи. Они помогут закрепить понимание типов данных, операций над переменными, работы со строками, коллекциями и особенностями памяти в Python.\n",
    "\n",
    "---\n",
    "\n",
    "## Задание 1: Приветствие пользователя\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Запросите у пользователя его имя и возраст.\n",
    "- Выведите сообщение с использованием f-строки: \"Привет, _имя_! Тебе _возраст_ лет.\"\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Введите ваше имя: Алиса\n",
    "Введите ваш возраст: 20\n",
    "Привет, Алиса! Тебе 20 лет.\n",
    "```\n",
    "\n",
    "---"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Привет Алёна! Тебе 20 лет.\n"
     ]
    }
   ],
   "source": [
    "import sys\n",
    "\n",
    "name = input('Введите ваше имя: ')\n",
    "while (not(name.isalpha())):\n",
    "    if (name == '_exit'): sys.exit()\n",
    "    print('Имя должно состоять только их букв')\n",
    "    name = input('Введите ваше имя: ')\n",
    "age = input('Введите ваш возраст: ')\n",
    "while (not(age.isdigit())):\n",
    "    if (age == '_exit'): sys.exit()\n",
    "    print('Возраст должен содержать только цифры')\n",
    "    age = input('Введите ваш возраст: ')\n",
    "print(f'Привет {name}! Тебе {age} лет.')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 2: Сумма и произведение чисел\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Запросите у пользователя два числа (целых или вещественных).\n",
    "- Вычислите и выведите их сумму и произведение.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Введите первое число: 5\n",
    "Введите второе число: 3\n",
    "Сумма чисел: 8\n",
    "Произведение чисел: 15\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Сумма чисел: 3.5\n",
      "Произведение чисел: 3.0\n"
     ]
    }
   ],
   "source": [
    "import sys\n",
    "\n",
    "def read_number(str, f):\n",
    "    while (str!= 'q'):\n",
    "        p = str.find('.')\n",
    "        if (p==-1):\n",
    "            if (str.isdigit()):\n",
    "                return int(str), f\n",
    "        elif (str[:p].isdigit() and str[p+1:].isdigit()):\n",
    "            return float(str), 0\n",
    "        str = input('Введите правильное число, состоящее только из цифр')\n",
    "    sys.exit()\n",
    "\n",
    "s = input('Введите первое число: ')\n",
    "flag = 1\n",
    "a, flag = read_number(s, flag)\n",
    "s = input('Введите второе число: ')\n",
    "\n",
    "b, flag = read_number(s, flag)\n",
    "\n",
    "sum = a+b\n",
    "pr = a*b\n",
    "if (flag == 0):\n",
    "    print(f'Сумма чисел: {sum:.2}')\n",
    "    print(f'Произведение чисел: {pr:.2}')\n",
    "else:\n",
    "    print(f'Сумма чисел: {sum}')\n",
    "    print(f'Произведение чисел: {pr}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 3: Преобразование типов\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Запросите у пользователя число в виде строки.\n",
    "- Преобразуйте эту строку в целое число и выведите его квадрат.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Введите число: 7\n",
    "Квадрат числа: 49\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Квадрат числа: 144\n"
     ]
    }
   ],
   "source": [
    "import sys\n",
    "\n",
    "def read_number(str):\n",
    "    while (str!= 'q'):\n",
    "        if str.isdigit():\n",
    "            return int(str)\n",
    "        str = input('Введите правильное число, состоящее только из цифр')\n",
    "    sys.exit()\n",
    "\n",
    "s = input('Введите число: ')\n",
    "print('Квадрат числа:', read_number(s)**2)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 4: Работа со списками\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте список из трех ваших любимых цветов.\n",
    "- Добавьте в этот список еще один цвет.\n",
    "- Замените второй элемент списка на \"черный\".\n",
    "- Выведите итоговый список.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Изначальный список: [\"красный\", \"синий\", \"зелёный\"]\n",
    "Итоговый список: [\"красный\", \"черный\", \"зелёный\", \"желтый\"]\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Изначальный список: ['red', 'green', 'blue']\n",
      "Итоговый список: ['red', 'чёрный', 'blue', 'pink']\n"
     ]
    }
   ],
   "source": [
    "c = ['red', 'green', 'blue']\n",
    "print('Изначальный список:',c)\n",
    "c.append('pink')\n",
    "c[1] = 'чёрный'\n",
    "print('Итоговый список:', c)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 5: Индексация строк\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Запросите у пользователя любое слово.\n",
    "- Выведите первый и последний символ этого слова.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Введите слово: Python\n",
    "Первый символ: P\n",
    "Последний символ: n\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Первый символ: P\n",
      "Последний сивол: n\n"
     ]
    }
   ],
   "source": [
    "s = input('Введите слово')\n",
    "print('Первый символ:', s[0])\n",
    "print('Последний сивол:', s[-1])"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 6: Словарь персональных данных\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте словарь с ключами: \"name\", \"age\", \"city\".\n",
    "- Заполните его данными о себе.\n",
    "- Выведите фразу, используя данные из словаря: \"Меня зовут _name_, мне _age_ лет, я из города _city_.\"\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Меня зовут Иван, мне 16 лет, я из города Москва.\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Меня зовут Sasha, мне 16 лет, я из гоорода Moscow\n"
     ]
    }
   ],
   "source": [
    "my_inf = {\n",
    "    'name': 'Sasha',\n",
    "    'age': 16,\n",
    "    'city': 'Moscow'\n",
    "}\n",
    "\n",
    "print(f'Меня зовут {my_inf['name']}, мне {my_inf['age']} лет, я из гоорода {my_inf[\"city\"]}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 7: Уникальные элементы множества\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте список чисел с повторяющимися значениями.\n",
    "- Преобразуйте этот список во множество, чтобы получить уникальные элементы.\n",
    "- Выведите полученное множество.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Список: [1, 2, 3, 2, 1, 4]\n",
    "Множество: {1, 2, 3, 4}\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Список: [1, 2, 3, 2, 4, 1]\n",
      "Множество: {1, 2, 3, 4}\n"
     ]
    }
   ],
   "source": [
    "l = [1, 2, 3, 2, 4, 1]\n",
    "print('Список:', l)\n",
    "print('Множество:', set(l))"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 8: Конкатенация строк\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Запросите у пользователя два слова.\n",
    "- Соедините их в одну строку с пробелом между ними.\n",
    "- Повторите полученную строку 3 раза и выведите результат.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Введите первое слово: Доброе\n",
    "Введите второе слово: утро\n",
    "Результат: Доброе утро Доброе утро Доброе утро\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Результат Black Jack Black Jack Black Jack \n"
     ]
    }
   ],
   "source": [
    "a = input('Введите первое слово: ')\n",
    "b = input('Введите второе слово: ')\n",
    "s = a + ' ' + b + ' '\n",
    "print('Результат', s*3)"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 9: Изменение кортежа\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте кортеж из трёх любых чисел.\n",
    "- Попытайтесь изменить второй элемент кортежа на другое число.\n",
    "- Объясните, что произошло и почему.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "metadata": {},
   "outputs": [
    {
     "ename": "TypeError",
     "evalue": "'tuple' object does not support item assignment",
     "output_type": "error",
     "traceback": [
      "\u001b[31m---------------------------------------------------------------------------\u001b[39m",
      "\u001b[31mTypeError\u001b[39m                                 Traceback (most recent call last)",
      "\u001b[36mCell\u001b[39m\u001b[36m \u001b[39m\u001b[32mIn[11]\u001b[39m\u001b[32m, line 2\u001b[39m\n\u001b[32m      1\u001b[39m s = (\u001b[32m1\u001b[39m, \u001b[32m2\u001b[39m ,\u001b[32m3\u001b[39m)\n\u001b[32m----> \u001b[39m\u001b[32m2\u001b[39m \u001b[43ms\u001b[49m\u001b[43m[\u001b[49m\u001b[32;43m1\u001b[39;49m\u001b[43m]\u001b[49m = \u001b[32m0\u001b[39m\n\u001b[32m      4\u001b[39m \u001b[38;5;66;03m# Кортеж неизменяем\u001b[39;00m\n",
      "\u001b[31mTypeError\u001b[39m: 'tuple' object does not support item assignment"
     ]
    }
   ],
   "source": [
    "s = (1, 2 ,3)\n",
    "s[1] = 0\n",
    "\n",
    "# Кортеж неизменяем"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 10: Длина коллекций\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте список из пяти элементов.\n",
    "- Создайте строку, состоящую из фразы \"Python - это круто!\".\n",
    "- Выведите длину списка и длину строки.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Длина списка: 5\n",
    "Длина строки: 17\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 13,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Длина списка: 5\n",
      "Длина строки: 22\n"
     ]
    }
   ],
   "source": [
    "l = ['sadas', '1', 212, 'sdf12', 5]\n",
    "s = 'Python is cool. Realy?'\n",
    "\n",
    "print('Длина списка:', len(l))\n",
    "print('Длина строки:', len(s))"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 11: Обмен значений переменных\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте две переменные `a` и `b`, присвоив им любые числовые значения.\n",
    "- Поменяйте значения переменных местами без использования дополнительной переменной.\n",
    "- Выведите новые значения переменных `a` и `b`.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Изначально: a = 3, b = 5\n",
    "После обмена: a = 5, b = 3\n",
    "```\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 15,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Изначально: a = 1, b = 3\n",
      "После обмена: a = 3, b = 1\n",
      "После второго обмена: a = 1, b = 3\n"
     ]
    }
   ],
   "source": [
    "a, b = 1, 3\n",
    "print(f'Изначально: a = {a}, b = {b}')\n",
    "a, b = b, a\n",
    "print(f'После обмена: a = {a}, b = {b}')\n",
    "a = a^b\n",
    "b = a^b\n",
    "a = a^b\n",
    "print(f'После второго обмена: a = {a}, b = {b}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 12: Форматирование чисел\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте переменную `pi` и присвойте ей значение 3.14159265.\n",
    "- Выведите значение `pi`, округлив его до двух знаков после запятой, используя f-строку.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Число пи приблизительно равно 3.14\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 16,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Число пи приблизительно равно 3.14\n"
     ]
    }
   ],
   "source": [
    "pi = 3.14159265\n",
    "print(f'Число пи приблизительно равно {pi:.2f}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 13: Проверка типов данных\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте переменные разных типов: целое число, вещественное число, строку и логическое значение.\n",
    "- Используйте функцию `type()`, чтобы вывести тип каждой переменной.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Тип переменной x: <class 'int'>\n",
    "Тип переменной y: <class 'float'>\n",
    "Тип переменной z: <class 'str'>\n",
    "Тип переменной is_valid: <class 'bool'>\n",
    "```\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 17,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Тип переменной a: <class 'int'>\n",
      "Тип переменной b: <class 'float'>\n",
      "Тип переменной c: <class 'str'>\n",
      "Тип переменной d: <class 'bool'>\n"
     ]
    }
   ],
   "source": [
    "a = 6\n",
    "b = 4.84\n",
    "c = 'олд9'\n",
    "d = True\n",
    "\n",
    "print(f'Тип переменной a: {type(a)}')\n",
    "print(f'Тип переменной b: {type(b)}')\n",
    "print(f'Тип переменной c: {type(c)}')\n",
    "print(f'Тип переменной d: {type(d)}')"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 14: Изменение списков и их копий\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте список `original_list` с элементами `[1, 2, 3]`.\n",
    "- Создайте переменную `copied_list` и присвойте ей значение `original_list`.\n",
    "- Добавьте элемент `4` в список `original_list`.\n",
    "- Выведите оба списка и объясните результат.\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 19,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "[1, 2, 3, 5]\n",
      "[1, 2, 3, 5]\n"
     ]
    }
   ],
   "source": [
    "original_list = [1,2,3]\n",
    "copied_list = original_list\n",
    "original_list.append(5)\n",
    "\n",
    "print(original_list)\n",
    "print(copied_list)\n",
    "\n",
    "# Обе перменные ссылают на один и тот список\n",
    "# Чтобы это были разние списки необходимо использовать copy"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Задание 15: Работа с NoneType\n",
    "\n",
    "**Описание:**\n",
    "\n",
    "- Создайте переменную `result` и не присваивайте ей никакого значения (или присвойте `None`).\n",
    "- Проверьте, равна ли переменная `result` значению `None`.\n",
    "- Выведите соответствующее сообщение.\n",
    "\n",
    "**Пример:**\n",
    "\n",
    "```\n",
    "Результат не определён.\n",
    "```"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 20,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Результат не определен.\n"
     ]
    }
   ],
   "source": [
    "result = None\n",
    "if(result == None):\n",
    "    print('Результат не определен.')"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.6"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
