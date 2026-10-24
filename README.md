<div align="center">

# 💻 LeetCode Solutions & Algorithms:

Коллекция решений задач на платформе [LeetCode](https://leetcode.com/) с акцентом на чистый код, анализ асимптотической сложности и разбор оптимальных алгоритмических паттернов.

<!-- Замените YOUR_LEETCODE_USERNAME на ваш никнейм на LeetCode -->
<!-- Дополнительно можно добавить &ext=heatmap или &ext=activity для отображения активности -->
[![LeetCode Stats](https://leetcard.jacoblin.cool/YOUR_LEETCODE_USERNAME?theme=dark&font=Ubuntu&ext=heatmap)](https://leetcode.com/u/YOUR_LEETCODE_USERNAME/)

<br/>

[![Profile](https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/YOUR_LEETCODE_USERNAME/)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)](#)
[![SQL](https://img.shields.io/badge/SQL-PostgreSQL%20|%20MySQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](#)
[![TypeScript/JS](https://img.shields.io/badge/JS%20/%20TS-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-2ea44f?style=for-the-badge)](LICENSE)

</div>

---

## 🧭 Оглавление:

- [📊 Прогресс решений](#-прогресс-решений)
- [🧠 Алгоритмические паттерны](#-алгоритмические-паттерны)
- [🗂 Структура репозитория](#-структура-репозитория)
- [📌 Избранные задачи](#-избранные-задачи)
- [🧪 Локальный запуск и тесты](#-локальный-запуск-и-тесты)
- [🛠 Автоматическая синхронизация](#-автоматическая-синхронизация)
- [🚀 В планах (Roadmap)](#-в-планах-roadmap)
- [🚀 В планах (Roadmap)

---

## 📊 Прогресс решений:

<!-- Эту таблицу можно обновлять вручную или через GitHub Actions -->

| Категория | Всего решено | Easy 🟢 | Medium 🟡 | Hard 🔴 | Директория |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Algorithms** | 0 | 0 | 0 | 0 | [`/Algorithms`](./Algorithms) |
| **Database (SQL)** | 0 | 0 | 0 | 0 | [`/Database`](./Database) |
| **Pandas** | 0 | 0 | 0 | 0 | [`/pandas`](./pandas) |
| **JavaScript / TS** | 0 | 0 | 0 | 0 | [`/JavaScript`](./JavaScript) |
| **Concurrency** | 0 | 0 | 0 | 0 | [`/Concurrency`](./Concurrency) |
| **Shell** | 0 | 0 | 0 | 0 | [`/Shell`](./Shell) |
| **Итого** | **0** | **0** | **0** | **0** | — |

---

## 🧠 Алгоритмические паттерны:

Быстрая навигация 
по ключевым темам и методам решения задач:

| Паттерн / Тема | Описание и применение | Типичная сложность |
| :--- | :--- | :---: |
| **Two Pointers** | Поиск пар, работа с отсортированными массивами и палиндромами | $\mathcal{O}(N)$ |
| **Sliding Window** | Поиск оптимальных подмассивов или подстрок (фиксированных и динамических) | $\mathcal{O}(N)$ |
| **Binary Search** | Поиск в отсортированных данных и бинарный поиск по ответу | $\mathcal{O}(\log N)$ |
| **Prefix Sum & Hashing** | Быстрый подсчет сумм на отрезках и поиск комплементарных значений | $\mathcal{O}(N)$ |
| **Trees & Graphs (BFS/DFS)** | Обход деревьев, графов, поиск кратчайших путей, топологическая сортировка | $\mathcal{O}(V + E)$ |
| **Dynamic Programming** | Задачи оптимизации и подсчета способов с перекрывающимися подзадачами | $\mathcal{O}(N^2)$, $\mathcal{O}(N \cdot W)$ |
| **Heap / Priority Queue** | Поиск $K$ наибольших/наименьших элементов, слияние потоков, алгоритм Дейкстры | $\mathcal{O}(N \log K)$ |
| **Backtracking** | Генерация перестановок, комбинаций и поиск с возвратом | $\mathcal{O}(2^N)$, $\mathcal{O}(N!)$ |

---

## 🗂 Структура репозитория:

Репозиторий разделен по основным направлениям платформы. Каждое решение именуется по формату `XXXX-problem-slug.ext` для удобной сортировки:

```text
.
├── Algorithms/       # Алгоритмы и структуры данных (Arrays, DP, Graphs, Trees и др.)
├── Concurrency/      # Многопоточность, примитивы синхронизации и асинхронность
├── Database/         # Решения на SQL (PostgreSQL / MySQL): окна, CTE, агрегации
├── JavaScript/       # Специфика JS/TS (Closures, Promises, Generators, Event Loop)
├── Shell/            # Скрипты автоматизации и парсинга текста на Bash (awk, sed, grep)
├── pandas/           # Обработка, очистка и векторная трансформация табличных данных
├── tests/            # Модульные тесты для локальной проверки решений
└── README.md
```

### 📝 Стандарт оформления решения:

Каждое решение включает метаданные задачи, описание идеи алгоритма и оценку сложности по времени и памяти:

```python
"""
ID: 0001
Название: Two Sum
Сложность: Easy
Ссылка: https://leetcode.com/problems/two-sum/
Паттерн: Hash Table

Идея решения:
Проходим по массиву один раз, сохраняя в хеш-таблицу уже встреченные числа и их индексы.
Для каждого элемента проверяем, есть ли в таблице дополнение (target - num).

Временная сложность (Time Complexity): O(N)
Пространственная сложность (Space Complexity): O(N)
"""

class Solution:
    def twoSum(self, nums: list[int], target: int) -> list[int]:
        lookup: dict[int, int] = {}
        for idx, num in enumerate(nums):
            diff = target - num
            if diff in lookup:
                return [lookup[diff], idx]
            lookup[num] = idx
        return []
```

---

## 📌 Избранные задачи:

<details open>
<summary><b>🔥 Algorithms: Классические задачи</b></summary>
<br/>

| # | Название | Решение | Паттерн | Сложность | Время | Память |
|:---:|:---|:---:|:---|:---:|:---:|:---:|
| 0001 | [Two Sum](https://leetcode.com/problems/two-sum/) | [Python](./Algorithms/0001-two-sum.py) | `Hash Map` | 🟢 Easy | $\mathcal{O}(N)$ | $\mathcal{O}(N)$ |
| 0015 | [3Sum](https://leetcode.com/problems/3sum/) | [Python](./Algorithms/0015-3sum.py) | `Two Pointers` | 🟡 Medium | $\mathcal{O}(N^2)$ | $\mathcal{O}(1)$ |
| 0042 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) | [Python](./Algorithms/0042-trapping-rain-water.py) | `Two Pointers` | 🔴 Hard | $\mathcal{O}(N)$ | $\mathcal{O}(1)$ |
| 0146 | [LRU Cache](https://leetcode.com/problems/lru-cache/) | [Python](./Algorithms/0146-lru-cache.py) | `Design / LinkedList` | 🟡 Medium | $\mathcal{O}(1)$ | $\mathcal{O}(C)$ |
| 0200 | [Number of Islands](https://leetcode.com/problems/number-of-islands/) | [Python](./Algorithms/0200-number-of-islands.py) | `DFS / BFS` | 🟡 Medium | $\mathcal{O}(M \cdot N)$ | $\mathcal{O}(M \cdot N)$ |

</details>

<details>
<summary><b>🗄️ Database: SQL</b></summary>
<br/>

| # | Название | Решение | Тема | Сложность | Диалект |
|:---:|:---|:---:|:---|:---:|:---:|
| 0175 | [Combine Two Tables](https://leetcode.com/problems/combine-two-tables/) | [SQL](./Database/0175-combine-two-tables.sql) | `LEFT JOIN` | 🟢 Easy | PostgreSQL / MySQL |
| 0184 | [Department Highest Salary](https://leetcode.com/problems/department-highest-salary/) | [SQL](./Database/0184-department-highest-salary.sql) | `Window Functions` | 🟡 Medium | PostgreSQL |
| 0185 | [Department Top Three Salaries](https://leetcode.com/problems/department-top-three-salaries/) | [SQL](./Database/0185-department-top-three-salaries.sql) | `DENSE_RANK()` | 🔴 Hard | PostgreSQL |

</details>

<details>
<summary><b>🐼 Data Science: Pandas</b></summary>
<br/>

| # | Название | Решение | Тема | Сложность |
|:---:|:---|:---:|:---|:---:|
| 2877 | [Create a DataFrame from List](https://leetcode.com/problems/create-a-dataframe-from-list/) | [Python](./pandas/2877-create-a-dataframe-from-list.py) | `Data Structure` | 🟢 Easy |
| 2889 | [Reshape Data: Pivot](https://leetcode.com/problems/reshape-data-pivot/) | [Python](./pandas/2889-reshape-data-pivot.py) | `Table Reshaping` | 🟢 Easy |

</details>

<details>
<summary><b>⚡ JavaScript & Concurrency</b></summary>
<br/>

| # | Название | Решение | Категория | Сложность |
|:---:|:---|:---:|:---|:---:|
| 1114 | [Print in Order](https://leetcode.com/problems/print-in-order/) | [Python](./Concurrency/1114-print-in-order.py) | `Threading / Locks` | 🟢 Easy |
| 2622 | [Cache With Time Limit](https://leetcode.com/problems/cache-with-time-limit/) | [JS](./JavaScript/2622-cache-with-time-limit.js) | `Timers / Closures` | 🟡 Medium |
| 2637 | [Promise Time Limit](https://leetcode.com/problems/promise-time-limit/) | [JS](./JavaScript/2637-promise-time-limit.js) | `Promises` | 🟡 Medium |

</details>

---

## 🧪 Локальный запуск и тесты::

Для запуска решений и проверки краевых случаев (edge cases) локально:

```bash
# Клонирование репозитория
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME

# Установка зависимостей для тестирования (опционально)
pip install pytest pandas

# Запуск всех тестов
pytest
```

---

## 🛠 Автоматическая синхронизация:

Репозиторий поддерживает автоматическую выгрузку решений из браузера сразу после успешного прохождения всех тестов (`Accepted`):

- **[LeetHub 3.0](https://github.com/raphaelheinz/LeetHub-3.0)** / **[LeetSync](https://github.com/TargetParking/LeetSync)** — браузерные расширения для синхронизации кода и описания задач с GitHub.
- **GitHub Actions** — автоматическое обновление счетчиков и таблиц решенных задач при пуше новых коммитов.

---

## 🚀 В планах (Roadmap):

- [x] Оформить базовую структуру репозитория и бейджи со статистикой.
- [x] Разработать единый шаблон решений с оценкой $\mathcal{O}$-сложности.
- [ ] Настроить GitHub Action для авто-генерации таблицы прогресса.
- [ ] Добавить краткие конспекты (`Cheatsheets`) по основным структурам данных.
- [ ] Покрыть ключевые алгоритмические задачи локальными `pytest`-тестами.

---

<div align="center">

*Если этот репозиторий оказался вам полезен, поддержите его звездой ⭐️!*

</div>
