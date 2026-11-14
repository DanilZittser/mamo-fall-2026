# Методы и алгоритмы машинного обучения

Материалы дисциплины «Методы и алгоритмы машинного обучения» для студентов 3 курса направления 09.03.03 «Прикладная информатика» ТюмГУ, осенний семестр 2026 года. Преподаватель — Данил Зитцер (d.k.zitcer@utmn.ru).

Теория курса опирается на книгу Орельена Жерона «_Прикладное машинное обучение с помощью Scikit-Learn, Keras и TensorFlow_» (русский перевод 2020 года, 2-е издание, ISBN _978-5-907203-33-4_ (рус.)).

## Структура репозитория

- `lectures/` — PDF-презентации лекций, по папке на лекцию;
- `practices/` — практические занятия: по Jupyter-блокноту на занятие;
- `self-study/` — самостоятельные работы на практиках: по Jupyter-блокноту на работу;
- `requirements.txt` — зависимости для запуска блокнотов с точными версиями.

## Лекции

| № | Тема | Книга | Презентация |
|---|---|---|---|
| 02 | Этапы проекта машинного обучения | прил. Б | [PDF](lectures/02-end-to-end-project/02-end-to-end-project.pdf) |
| 03 | Классификация и метрики качества | гл. 3 | [PDF](lectures/03-classification/03-classification.pdf) |
| 04 | Обучение линейной регрессии | гл. 4 | [PDF](lectures/04-training-linear-regression/04-training-linear-regression.pdf) |

## Практики

| №  | Тема                             | Материал |
|----|----------------------------------|---|
| 01 | Окружение, репозиторий, git      | [README с командами занятия](practices/01-python-environment-and-git/README.md) |
| 02 | Минимум Python, NumPy, pandas    | [02-python-data-stack.ipynb](practices/02-python-data-stack/02-python-data-stack.ipynb) |
| 03 | Полный проект машинного обучения | [03-end-to-end-project.ipynb](practices/03-end-to-end-project/03-end-to-end-project.ipynb) |
| 04 | Задача Классификация (MNIST)     | [04-classification.ipynb](practices/04-classification/04-classification.ipynb) |
| 05 | Обучение лин. моделей (часть 1)  | [05-model-training.ipynb](practices/05-model-training/05-model-training.ipynb) |

## Самостоятельные работы

Блокнот самостоятельной работы выполняется на практике и защищается преподавателю. Защищать можно любое число заданий — от одного до всех; баллы ставятся только за защищённые задания. Правила и критерии — в начале каждого блокнота.

| № | Тема | Лекция | Блокнот |
|---|---|---|---|
| 01 | Метрики качества классификации | 03 | [01-classification-metrics.ipynb](self-study/01-classification-metrics.ipynb) |
| 02 | Обучение линейной регрессии | 04 | [02-linear-regression.ipynb](self-study/02-linear-regression.ipynb) |
| 03 | Градиентный спуск | 04 | [03-gradient-descent.ipynb](self-study/03-gradient-descent.ipynb) |
| 04 | Регуляризация и логистическая регрессия | 05 | [04-regularization-logistic.ipynb](self-study/04-regularization-logistic.ipynb) |

## Как запустить блокноты

На занятиях используется **Python 3.8**. Подробно каждая команда разобрана в [практике 01](practices/01-python-environment-and-git/README.md).

```bash
git clone git@github.com:DanilZittser/mamo-fall-2026.git  # скачать репозиторий
cd mamo-fall-2026/
python3 -m venv venv  # создать виртуальное окружение
source venv/bin/activate  # активировать окружение; в Windows: venv\Scripts\activate
pip install -r requirements.txt  # установить зависимости
jupyter notebook  # открыть Jupyter в браузере и выбрать блокнот в practices/ или self-study/
```

Чтобы получить новые материалы, в папке репозитория выполните `git pull`. Блокноты сами создают рядом с собой папку `data/` с наборами данных.
