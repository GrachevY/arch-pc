---
## Front matter
title: "Отчёт по лабораторной работе 2"
subtitle: "дисциплина: Архитектура компьютеров"
author: "Грачев Я. М. НПИбд-01-24"

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
lot: true # List of tables
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Ознакомиться с системой контроля версий Git, настроить его, завести репозиторий на сайте github и скинуть в него свои отчеты по лабораторным работам.

# Выполнение лабораторной работы

## Базовая настройка git

Делаем предварительную конфигурацию git. (рис. [-@fig:001])

![Задаем имя и email репозитория](image/01.png){ #fig:001 width=70%, height=70% }

Настраиваем utf-8 в выводе сообщения git. (рис. [-@fig:002])

![Настраиваем utf-8](image/02.png){ #fig:002 width=70%, height=70% }

Задаём имя начальной ветки. (рис. [-@fig:003])

![Задаем имя начальной ветки, как master](image/03.png){ #fig:003 width=70%, height=70% }

![Устанавливаем настройку autocrlf](image/04.png){ #fig:004 width=70%, height=70% }

![Устанавливаем параметр safecrlf](image/05.png){ #fig:005 width=70%, height=70% }

## Создание SSH ключа.

![Генерируем пару ключей](image/06.png){ #fig:006 width=70%, height=70% }

![Копируем ключ из локальной консоли в буфер обмена](image/07.png){ #fig:007 width=70%, height=70% }

Заходим в свой аккаунт на сайте github. 
Переходим в настройки.(рис. [-@fig:008]])

![Добавляем скопированный ключ и указываем имя ключа(Title)](image/08.png){ #fig:008 width=70%, height=70% }

![Проверяем добавление ключа](image/09.png){ #fig:009 width=70%, height=70% }

## Создание рабочего пространства и репозитория курса на основе шаблона.

Открываем терминал

![Создаем каталог для предмета “Архитектура компьютера”](image/10.png){ #fig:010 width=70%, height=70% }

## Создание репозитория курса

Переходим на страницу репозитория с шаблоном.

![Создаем репозиторий по шаблону и называем его “study_2024–2025_arh-pc”](image/11.png){ #fig:011 width=70%, height=70% }

Открываем терминал.

![Переходим в каталог курса](image/12.png){ #fig:012 width=70%, height=70% }

![Клонируем созданный репозиторий](image/13.png){ #fig:013 width=70%, height=70% }

## Настройка каталога курса

![Переходим в каталог курса](image/14.png){ #fig:014 width=70%, height=70% }

![Удаляем лишние файлы](image/15.png){ #fig:015 width=70%, height=70% }

![Создаем необходимые каталоги](image/16.png){ #fig:016 width=70%, height=70% }

![Отслеживаем файл и записываем изменения в репозиторий](image/17.png){ #fig:017 width=70%, height=70% }

![Отправляем данные в репозиторий](image/18.png){ #fig:018 width=70%, height=70% }

![Проверяем выполнение команд](image/19.png){ #fig:019 width=70%, height=70% }

![Загружаем в репозиторий отчет по первой лабораторной работе в папку lab01 (команда git push)](image/20.png){ #fig:020 width=70%, height=70% }

# Выводы

Мы познакомились с системой контроля git, выучили команды для работы с ним, создали свой репозиторий на платформе github, где в последствии будут храниться все будущие отчёты по лабораторным работам.а также приобрела практические навыки по работе с системой git.