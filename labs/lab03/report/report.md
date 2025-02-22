---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Имитационное моделирование"
author: "Волгин Иван"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: false # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Изучить теорию про СМО и применить полученные знания на практике.

# Задание

1. Написать модель СМО на NS-2.
2. Построить график в GNUplot.

# Выполнение лабораторной работы

1. Я приступил к выполнеию первого задания, где нужно было написать модель СМО на NS-2. Код модели можно увидеть на (рис. [-@fig:001]) (рис. [-@fig:002]).

![СМО](image/1.png){#fig:001 width=70%}

![СМО](image/2.png){#fig:002 width=70%}

В итоге я получил следующие результаты (рис. [-@fig:003]). Теоретическая вероятность потери очень мала, почти 0. Средняя длина очереди получилась 9.

![Полученные результаты](image/3.png){#fig:003 width=70%}

2. Вторым заданием было построить график и для начала я созал файл с помощью команды touch graph_plot (рис. [-@fig:003]).
Затем я написал код файла (рис. [-@fig:004]).

![Создание файла](image/4.png){#fig:004 width=70%}

![Код файла](image/5.png){#fig:005 width=70%}

Когда все было готово, файлу нужно было добавить право на выполнение командой chmod +x graph_plot (рис. [-@fig:006]). После этого я запустил файл и получил результат в виде графика (рис. [-@fig:007])

![Добавление прав файлу](image/6.png){#fig:006 width=70%}

![Получившийся график](image/7.png){#fig:007 width=70%}

# Выводы

В ходе выполение лабораторной работы я ознакомился с СМО и сделал несколько практических заданий, что позволило мне лучше понять тему.

