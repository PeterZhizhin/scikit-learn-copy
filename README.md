# Реализация алгоритма спектральных вложений Грассмана-Штифеля
## Жижин Петр Николаевич 152 группа

Целью данного проекта является модернизация библиотеки scikit-learn с целью добавления нового функционала в раздел manifold библиотеки.

### Актуальность решаемой задачи

Библиотека scikit-learn является одной из самых популярных библиотек машинного обучения, которая используется большим 
числом специалистов по анализу данных по всему миру.
На данный момент в библиотеки реализованы некоторые алгоритмы снижения размерности среди которых есть в том числе и алгоритмы
MDS и IsoMap.

Несмотря на большую значимость библиотеки, в нее не входят для некоторых алгоритмов отсутствует возможность построения
вложения для точек, не входящих в обучаюющую выборку (построения out-of-sample вложения). Так же в ней нет алгоритмов
для получения исходных точек из пространства вложения (reverse out-of-sample).

### Обзор использованных технологических решений

В рамках решения задачи были использованы следующие технологические решения:

* Встроенные в scikit-learn алгоритмы
* Python 2, Python 3
* Cython 2, Cython 3

Выбор данных технологий обусловлен тем, что задача решается в рамках уже существующей библиотеки с существующими
зависимостями.

### План решения задачи

* Реализовать алгоритм для построения out-of-sample вложения для алгоритмов MDS и IsoMap.
* Реализовать алгоритм reverse out-of-sample для алгоритмов MDS и IsoMap.
