---
## Front matter
title: "Лабораторная работа №12"
subtitle: "Имитационное моделирование"
author: "Волгин Иван Алексеевич"

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

Изучить пример моделирования простого протокола передачи данных и построить его самостоятельно опираясь на данный пример

# Задание

1. Изучить пример моделирования простого протокола передачи данных
2. Построить самостоятельно модель
3. Вычислить пространство состояний
4. Построить граф пространства состояний

# Выполнение лабораторной работы

Для начала я изучил пример моделирования постого протокола передачи данных. Затем перешел к самостоятельному построению. Для начала нужно было задать декларации модели (рис. [-@fig:001]).

![Декларации модели](image/1.png){#fig:001 width=70%}

Вторым шагом я строю начальный граф и правильно настраиваю все значения и типы состояний (рис. [-@fig:002]).

![Начальный граф](image/2.png){#fig:002 width=70%}

Далее к начальному графу добавляем промежуточные состояния (рис. [-@fig:003])

![Промежуточные состояния](image/3.png){#fig:003 width=70%}

Затем нужно было добавить дополнительные декларации (рис. [-@fig:004])

![Дополнительные декларации](image/4.png){#fig:004 width=70%}

Следующим шагом я заканчиваю строить граф и получаю модель простого протокола передачи данных (рис. [-@fig:005])

![модель простого протокола передачи данных](image/5.png){#fig:005 width=70%}

Чтобы удостовериться в правильности выполнения построения, я запустил модель и в результате получил полное сообщение, что свидетельствует об успешном построении (рис. [-@fig:006])

![Результат работы модели](image/6.png){#fig:006 width=70%}

Далее я перешел к выполнению упражнения, в котором нужно было вычислить пространство состояний, сформировать о нем отчет и построить граф пространства состояний. Сначала я сформировал отчет и проанализировал его (рис. [-@fig:007]). После этого я построил граф (рис. [-@fig:008])

![Отчет о пространстве состояний](image/7.png){#fig:007 width=70%}

![Граф пространства состояний](image/8.png){#fig:008 width=70%}

# Выводы

В ходе выполнения данной лабораторной работы, я изучил простую модель протокола передачи данных и построил его модель, а также проанализировал отчет о пространстве состояний и построил его граф.
