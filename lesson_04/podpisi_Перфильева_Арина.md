# Практикум «Младший разработчик: первая неделя»

МДК.01.01 · аннотации типов и окружение проекта

- Студент: Перфильева Арина
- Группа: РПО1
- Сдано: 30.10.2026, 13:46:13

## Рецензия

| Письмо | Результат | Баллы |
|---|---|---|
| Письмо 1 · рабочее место | 18 из 18 | 2 / 2 |
| Письмо 2 · подписи по заявкам | 0 из 10 | 0 / 4 |
| Письмо 3 · вызовы и подпись | 36 из 40 | 2 / 2 |
| Письмо 4 · подпись вручную | 3 из 4 | 1 / 2 |
| **Итого** | | **5 / 10 · удовлетворительно** |

- Рабочее место: все ответы верны.
- Подписи по заявкам: не решены заявки 1, 2, 3, 4, 5, 6, 7, 8, 9, 10. Повторите: какие данные нужны функции, а какие нет; словари и кортежи в аннотациях (глава 4.2, §2); порядок параметров со значением по умолчанию (глава 4.1, §3); запись X | None и объединение int | str (глава 4.2, §4–5); -> None у функции без результата (глава 4.2, §1).
- Вызовы и подпись: ошибки в подписях 2, 4, 5. Прочитайте разбор под каждой.
- Подпись вручную: не решена заявка 3.

## Письмо 1. Рабочее место

### Порядок команд — верно

1. `Распаковать архив и открыть папку проекта в VS Code: File → Open Folder, затем Terminal → New Terminal`
2. `python -m venv .venv`
3. `Активировать окружение: .venv\Scripts\activate в Windows или source .venv/bin/activate в macOS и Linux`
4. `python -m pip install -r requirements.txt`
5. `python main.py`

### Первый коммит — верно 10 из 10

| Файл | Ваш ответ | Верно |
|---|---|---|
| `main.py` | в репозиторий | ✓ |
| `app/calculator.py` | в репозиторий | ✓ |
| `tests/test_calculator.py` | в репозиторий | ✓ |
| `requirements.txt` | в репозиторий | ✓ |
| `README.md` | в репозиторий | ✓ |
| `.gitignore` | в репозиторий | ✓ |
| `.venv/` | на компьютере | ✓ |
| `__pycache__/` | на компьютере | ✓ |
| `app/__pycache__/calculator.cpython-312.pyc` | на компьютере | ✓ |
| `.env` | на компьютере | ✓ |

### Вопросы из чата — верно 7 из 7

| Вопрос | Ваша причина | Верно |
|---|---|---|
| 1. Денис | Пакет установлен в другой Python, не в окружение проекта | ✓ |
| 2. Лиза | Окружение не активно в этом терминале | ✓ |
| 3. Ксюша | Зависимости проекта не записаны в requirements.txt | ✓ |
| 4. Глеб | Нет правил .gitignore для окружения и кэша | ✓ |
| 5. Марат | Список зависимостей снят не в окружении проекта | ✓ |
| 6. Оля | VS Code использует другой интерпретатор, не из .venv | ✓ |
| 7. Тимур | Окружение перенесено с другого компьютера | ✓ |

## Письмо 2. Подписи по заявкам

### 1. Колледж «Северный» · электронный журнал — неверно

```python
def average_grade(group_number: str, student_name: str, grades: list[int]) -> float:
```

### 2. Колледж «Северный» · посещаемость — неверно

```python
def count_absences(teacher: str, marks: list[str], month: str) -> int:
```

### 3. Кофейня «Зерно» · касса — неверно

```python
def order_total(table_number: int, discount: int = 0, items: dict[str, int], barista: str) -> int:
```

### 4. Кофейня «Зерно» · постоянные гости — неверно

```python
def find_guest_phone(name: str, guests: dict[str, str], phone: str) -> str | None:
```

### 5. Фитнес-клуб «Пульс» · абонементы — неверно

```python
def is_membership_active(today: date, client_name: str, end_date: date, price: int) -> bool:
```

### 6. Книжный магазин «Переплёт» · склад — неверно

```python
def parse_quantity(warehouse: int, title: str, value: int | str) -> int:
```

### 7. Курьерская служба «Квартал» · отчёт за день — неверно

```python
def distance_bounds(distances: list[float], day: date, courier: str) -> tuple[float, float]:
```

### 8. Кофейня «Зерно» · печать чека — неверно

```python
def print_receipt(width: int = 32, cashier: str, lines: list[str]) -> None:
```

### 9. Колледж «Северный» · ведомость группы — неверно

```python
def average_by_student(journal: dict[str, list[int]], group_number: str) -> dict[str, float]:
```

### 10. Фитнес-клуб «Пульс» · карта клиента — неверно

```python
def format_name(last_name: str, first_name: str, birthday: date, middle_name: str | None = None) -> str:
```

## Письмо 3. Вызовы и подпись

| Подпись | Верно |
|---|---|
| `def average_grade(grades: list[int]) -> float:` | 8 из 8 |
| `def find_guest_phone(guests: dict[str, str], name: str) -> str \| None:` | 6 из 8 |
| `def format_name(last_name: str, first_name: str, middle_name: str \| None = None) -> str:` | 8 из 8 |
| `def parse_quantity(value: int \| str) -> int:` | 7 из 8 |
| `def print_receipt(lines: list[str], width: int = 32) -> None:` | 7 из 8 |

## Письмо 4. Подпись вручную

### 1. Колледж «Северный» · лучший студент — верно

```python
def best_student(averages: dict[str, float]) -> str | None:
```

### 2. Фитнес-клуб «Пульс» · бонусы — верно

```python
def add_bonus(balance: int, visits: int, is_vip: bool = False) -> int:
```

### 3. Курьерская служба «Квартал» · адреса — неверно

```python
def split_adress(adress: str) -> tuple[str, str]:
```

- имя функции split_adress, а в заявке split_address
- параметры: adress, а нужны address

### 4. Книжный магазин «Переплёт» · авторы — верно

```python
def unique_authors(books: list[tuple[str, str]]) -> set[str]:
```
