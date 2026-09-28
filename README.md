<div align="center">

# 💻 LeetCode Solutions & Algorithms

Коллекция решений задач на платформе [LeetCode](https://leetcode.com/) с акцентом на чистый код, разбор сложности и разные подходы к оптимизации.

<!-- Замените YOUR_LEETCODE_USERNAME на ваш никнейм на LeetCode -->
[![LeetCode Stats](https://leetcard.jacoblin.cool/YOUR_LEETCODE_USERNAME?theme=dark&font=Ubuntu)](https://leetcode.com/YOUR_LEETCODE_USERNAME/)

<br/>

[![Profile](https://img.shields.io/badge/LeetCode-Profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/YOUR_LEETCODE_USERNAME/)
[![Languages](https://img.shields.io/badge/Languages-Python%20|%20SQL%20|%20JS%20|%20Bash-blue?style=for-the-badge)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

</div>

---

## 📊 Прогресс решений

| Категория | Всего решено | Easy 🟢 | Medium 🟡 | Hard 🔴 |
| :--- | :---: | :---: | :---: | :---: |
| **Algorithms** | 0 | 0 | 0 | 0 |
| **Database (SQL)** | 0 | 0 | 0 | 0 |
| **Concurrency** | 0 | 0 | 0 | 0 |
| **JavaScript** | 0 | 0 | 0 | 0 |
| **Pandas** | 0 | 0 | 0 | 0 |
| **Shell** | 0 | 0 | 0 | 0 |
| **Итого** | **0** | **0** | **0** | **0** |

---

## 🗂 Структура репозитория

Каталог организован по направлениям. Каждое решение оформлено в отдельный файл или директорию с указанием номера задачи:

```text
.
├── Algorithms/       # Алгоритмы и структуры данных (DP, Graphs, Trees, Two Pointers)
├── Concurrency/      # Многопоточность и синхронизация потоков
├── Database/         # Решения на SQL (PostgreSQL / MySQL)
├── JavaScript/       # Задачи на специфику JS (Closures, Promises, Event Loop)
├── Shell/            # Скрипты автоматизации и парсинга на Bash
├── pandas/           # Обработка и трансформация данных средствами Pandas
└── README.md
```

### Формат оформления задачи

Каждое решение стремится следовать единому шаблону:

```python
"""
ID: 0001
Название: Two Sum
Сложность: Easy
Ссылка: https://leetcode.com/problems/two-sum/

Временная сложность (Time Complexity): O(n)
Пространственная сложность (Space Complexity): O(n)
"""

class Solution:
    def twoSum(self, nums: list[int], target: int) -> list[int]:
        lookup = {}
        for idx, num in enumerate(nums):
            diff = target - num
            if diff in lookup:
                return [lookup[diff], idx]
            lookup[num] = idx
        return []
```

---

## 📌 Примеры решенных задач

<details>
<summary><b>🔥 Algorithms: Топ задач</b></summary>

| # | Название | Решение | Сложность | Время | Память |
|:---:|:---|:---:|:---:|:---:|:---:|
| 0001 | [Two Sum](https://leetcode.com/problems/two-sum/) | [Python](./Algorithms/0001-two-sum.py) | `Easy` | $\mathcal{O}(N)$ | $\mathcal{O}(N)$ |
| 0015 | [3Sum](https://leetcode.com/problems/3sum/) | [Python](./Algorithms/0015-3sum.py) | `Medium` | $\mathcal{O}(N^2)$ | $\mathcal{O}(1)$ |
| 0042 | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/) | [Python](./Algorithms/0042-trapping-rain-water.py) | `Hard` | $\mathcal{O}(N)$ | $\mathcal{O}(1)$ |

</details>

<details>
<summary><b>🗄️ Database: SQL</b></summary>

| # | Название | Решение | Сложность | Диалект |
|:---:|:---|:---:|:---:|:---:|
| 0175 | [Combine Two Tables](https://leetcode.com/problems/combine-two-tables/) | [SQL](./Database/0175-combine-two-tables.sql) | `Easy` | MySQL |
| 0184 | [Department Highest Salary](https://leetcode.com/problems/department-highest-salary/) | [SQL](./Database/0184-department-highest-salary.sql) | `Medium` | PostgreSQL |

</details>

---

## 🛠 Автоматическая синхронизация

Репозиторий поддерживает автоматическую загрузку решений прямо из браузера с помощью одного из расширений:
- [LeetHub v2](https://github.com/raphaelheinz/LeetHub-2.0) — сохраняет решение сразу после успешного Submit.
- [GitHub Actions](.github/workflows/) — (опционально) скрипт для авто-обновления таблиц решенных задач.

---

## 🚀 В планах (To-Do)

- [x] Добавить бейджи со статистикой профиля LeetCode.
- [x] Добавить шаблон оформления решений с анализом Big-O.
- [ ] Настроить автоматическое обновление таблицы решенных задач через GitHub Actions.
- [ ] Добавить раздел с шпаргалками (Patterns / Cheatsheets: Sliding Window, Binary Search, Backtracking).
- [ ] Покрыть решения базовыми Unit-тестами (`pytest` / `unittest`).

---

<div align="center">

*Если репозиторий оказался полезен, поставь ⭐️!*

</div>
