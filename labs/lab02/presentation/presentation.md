---
## Front matter
lang: ru-RU
title: Лабораторная работа №2
subtitle: Имитационное моделирование
author:
  - Волгин И.А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 20 февраля 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="90%"}

  * Волгин Иван Алексеевич
  * Студент группы НФИбд-01-22 
  * Российский университет дружбы народов

:::
::::::::::::::

# Выполнение лабораторной работы

## Цели и задачи

Целью работы является исследовать протокл TCP и алгоритм управления очередью RED.

## Задание

- Создать пример сети с дисциплиной RED
- Выполнить дополнительное упражнение

## Код для модели сети из задания 1

![](image/1.png){#fig:001 width=95%}

## Графики размер окна и размера очереди

![](image/2.png){#fig:002 width=45%}
![](image/3.png){#fig:003 width=45%}

## Изменение типа TCP на Newreno

![](image/4.png){#fig:004 width=95%}

## Графики рамера окна и размера очереди с типом TCP Newreno 

![](image/5.png){#fig:005 width=45%}
![](image/6.png){#fig:006 width=45%}

## Изменение типа TCP на Vegas

![](image/7.png){#fig:007 width=95%}

## Графики рамера окна и размера очереди с типом TCP Vegas

![](image/8.png){#fig:008 width=45%}
![](image/9.png){#fig:009 width=45%}

## Код для изменения оформления

![](image/10.png){#fig:010 width=95%}

## Графики рамера окна и размера очереди с новым оформлением

![](image/11.png){#fig:011 width=45%}
![](image/12.png){#fig:012 width=45%} 

## Выводы

В ходе выполнения лабораторной работы я исследовал прокол TCP и алгоритм управления очередью RED
