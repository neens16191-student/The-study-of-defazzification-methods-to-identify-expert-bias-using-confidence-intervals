# The-study-of-defazzification-methods-to-identify-expert-bias-using-confidence-intervals

## English

### Overview
This repository contains the source code and dataset used in the study of how different defuzzification methods for triangular fuzzy numbers affect the detection of biased experts using confidence interval overlap.

The main focus of the research is the sensitivity of the confidence-interval-based expert bias detection method to the choice of defuzzification strategy applied to fuzzy expert evaluations.

### Repository Structure
- `main.py` — Python implementation of expert bias detection using confidence intervals, including multiple defuzzification strategies.
- `50_alternatives.json` — A fixed synthetic dataset of 50 alternatives with ground-truth labels indicating the biased expert for each alternative.

### Dataset Description
The dataset consists of 50 synthetic decision-making alternatives.  
Each alternative contains:
- A hierarchical criteria structure,
- Expert evaluations for each criterion,
- Expert and criterion weights,
- A `ground_truth` field specifying the expert that was intentionally generated as biased.

The dataset is generated once and reused for all experiments to ensure full reproducibility.

### Reproducibility
All experiments reported in the study are based exclusively on the provided dataset (`50_alternatives.json`).  
Users can reproduce the results by running `main.py` without modifying the dataset.

### Requirements
- Python 3.8+
- `numpy`
- `scipy`

---

## Русский

### Описание
Данный репозиторий содержит исходный код и датасет, использованные в исследовании влияния выбора функции дефаззификации треугольных нечетких чисел на выявление предвзятых экспертов методом пересечения доверительных интервалов.

Основное внимание в работе уделено анализу чувствительности алгоритма обнаружения предвзятости экспертов к различным стратегиям дефаззификации нечетких экспертных оценок.

### Структура репозитория
- `main.py` — реализация алгоритма выявления предвзятых экспертов с использованием доверительных интервалов и различных методов дефаззификации.
- `50_alternatives.json` — синтетический датасет из 50 альтернатив с указанием истинно предвзятого эксперта для каждой альтернативы.

### Описание датасета
Датасет состоит из 50 синтетических альтернатив принятия решений.  
Каждая альтернатива включает:
- Иерархическую структуру критериев,
- Оценки экспертов по каждому критерию,
- Веса экспертов и критериев,
- Поле `ground_truth`, указывающее на эксперта, который был сгенерирован как предвзятый.

Датасет генерируется один раз и используется во всех экспериментах, что обеспечивает воспроизводимость результатов.

### Воспроизводимость
Все экспериментальные результаты, представленные в работе, получены исключительно на основе датасета `50_alternatives.json`.  
Для воспроизведения экспериментов достаточно запустить файл `main.py` без изменения исходных данных.

### Требования
- Python 3.8+
- `numpy`
- `scipy`
