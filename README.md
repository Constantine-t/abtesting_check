# Final Project: Product Analytics & A/B Testing

[Читать на русском](#описание-на-русском)

---

## Project Overview

This repository contains solutions for a product analytics project. The main goals are:
- To analyze the results of an A/B test for a new payment mechanism;
- To evaluate student performance in an educational product;
- To automate metric recalculation and visualization.

All analysis is performed in a single Jupyter notebook.

### Data structure
- `groups.csv` – file with information about the user's belonging to the control or experimental group (A - control, B - target group);
- `groups_add.csv` – an additional user file that was sent to you 2 days after data transfer;
- `active_studs.csv` – a file with information about users who logged into the platform on the days of the experiment;
- `checks.csv` – a file with information on user fees on the days of the experiment.

### Structure

The project consists of three logical blocks:
1. **A/B Test Analytics** — Experiment analysis to assess the effect of the new payment mechanism;
2. **SQL Analytics** — Tasks for optimizing funnel and user segmentation using SQL;
3. **Python Automation & Visualization** — Scripts for automatic metric recalculation and plotting.

---

## 1. A/B Test Analytics

- Loaded and merged experimental data: control/test groups, payments, activity logs;
- Identified and justified key metrics: conversion to purchase, ARPU, ARPAU, retention, activity rate;
- Performed statistical analysis: compared groups by key metrics, assessed practical and statistical significance using appropriate tests (t-test, chi-square);
- Formulated recommendations on the launch of the new payment system.

---

## 2. SQL Analytics

- Wrote and explained SQL queries to:
    - Segment highly diligent students by month and discipline;
    - Calculate funnel metrics for all and active users, including those specifically active in math;
    - Measure ARPU, ARPAU, and conversion rates for various user segments.

---

## 3. Python Automation & Visualization

- Implemented a function to automatically update group memberships from `groups_add.csv` (handling column name differences), and recalculate metrics when new users appear;
- Built a reusable function to visualize resulting metrics as barplots and timelines.

---

## Usage

All solutions are in the Jupyter notebook:  
**`ab_testing_research.ipynb`**

### Requirements

- Python 3.9+;
- pandas, numpy, matplotlib, seaborn, scipy, statsmodels, jupyter.

### How to run

1. Place all CSV files in the notebook's working directory.
2. Open the notebook and run all cells.
3. For metric recalculation, update the group files and rerun the appropriate cells.

---

## Results & Recommendations

- Detailed statistical comparisons for each segment and metric;
- Practical recommendations for product management on whether to roll out the new payment system based on experiment outcomes.

---

# Описание на русском

[Read in English](#project-overview)

---

## Описание проекта

В этом репозитории находится решение учебного аналитического проекта, включающее:
- Анализ результатов A/B-теста новой механики оплаты;
- Оценку результатов студентов образовательного продукта;
- Автоматизацию пересчёта метрик и построения графиков.

Вся аналитика выполнена в одном Jupyter-ноутбуке.

### Структура данных
- `groups.csv` – файл с информацией о принадлежности пользователя к контрольной или экспериментальной группе (А – контроль, B – целевая группа);
- `groups_add.csv` – дополнительный файл с пользователями, который вам прислали спустя 2 дня после передачи данных;
- `active_studs.csv` – файл с информацией о пользователях, которые зашли на платформу в дни проведения эксперимента;
- `checks.csv` – файл с информацией об оплатах пользователей в дни проведения эксперимента.

---

## 1. Аналитика A/B-теста

- Загрузка и объединение данных: группы эксперимента, оплаты, активность пользователей;
- Определение и обоснование ключевых метрик: конверсия в оплату, ARPU, ARPAU, удержание, уровень активности;
- Статистический анализ: сравнение групп по метрикам, проверка практической и статистической значимости с помощью t-test и хи-квадрат;
- Формулировка рекомендации о внедрении новой механики оплаты.

---

## 2. SQL-Аналитика

- Оптимальные SQL-запросы для:
    - Сегментации очень усердных учеников по месяцам и предметам;
    - Расчёта метрик воронки по всем и активным пользователям, включая активных по математике;
    - Измерения ARPU, ARPAU и конверсии для разных сегментов.

---

## 3. Автоматизация и визуализация на Python

- Функция для автоматической подгрузки новых пользователей из `groups_add.csv` (с учётом возможных отличий в заголовках), обновления разметки и пересчёта всех метрик;
- Функция для построения графиков (barplot, timeline) по рассчитанным метрикам.

---

## Использование

Весь код и объяснения находятся в ноутбуке:  
**`ab_testing_research.ipynb`**

### Требования

- Python 3.9+;
- pandas, numpy, matplotlib, seaborn, scipy, statsmodels, jupyter.

### Как запустить

1. Поместите все csv-файлы в рабочую директорию ноутбука.
2. Откройте ноутбук и выполните все ячейки.
3. Для пересчёта метрик обновите файлы групп и выполните соответствующие ячейки заново.

---

## Результаты и рекомендации

- Подробное статистическое сравнение по каждому сегменту и метрике;
- Практические рекомендации по внедрению новой механики оплаты для менеджмента продукта.


