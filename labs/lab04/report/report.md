---
## Front matter
title: "Отчёт по лабораторной работе №4"
subtitle: "По архитектуре компьютера"
author: "Акопян Сатеник Манвеловна"

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
Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.
# Выполнение лабораторной работы
1. Перед выполнением лабораторной работы, нужно установить TeX Live, для этого
1.1. Скачиваем архив(рис. [-@fig:fig1])
![рисунок 1](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/1.png){ #fig:fig1 width=80% }
1.2. Распаковаваем архив (рис. [-@fig:fig2]) 
![рисунок 2](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/2.png){ #fig:fig2 width=80% }
1.3 Переходим в распакованную папку (рис.[-@fig:fig2])
1.4.Запускаем скрипт install-tl c root правами (рис.[-@fig:fig2]) 
![рисунок 3](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/3.png){ #fig:fig3 width=70% }
1.5. Добавляем /usr/local/texlive/2022/bin/x86_64-l/home/smakopyan/work/study/2022-2023/Архитеinux в PATH для текущей и будущих сессий.(рис.[-@fig:fig4]) 
![рисунок 4](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/4.png){ #fig:fig4 width=70% }
2. Также следует установить pandoc и pandoc-crossref, для этого
2.1.Скачиваем архивы с исходными файлами (рис.[-@fig:fig5]) (рис.[-@fig:fig6]) 
![рисунок 5](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/5.png){ #fig:fig5 width=70% } 
![рисунок 6](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/6.png){ #fig:fig6 width=70% }
2.2.Распаковываем архивы и копируем файлы pandoc и pandoc-crossref в каталог /usr/local/bin/ (рис.[-@fig:fig7]) (рис.[-@fig:fig8]) (рис.[-@fig:fig9]) 
![рисунок 7](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/7.png){ #fig:fig7 width=70% } 
![рисунок 8](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/8.png){ #fig:fig8 width=70% } 
![рисунок 9](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/9.png){ #fig:fig9 width=70% }
2.3. C помощью команды ls проверяем корректность выполненных действий  (рис.[-@fig:fig10])
![рисунок 10](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/10.png){ #fig:fig10 width=70% }
 3. Выполнение работы
3.1.В терминале переходим в каталог курса сформированный при выполнении лабораторной работы №3, обновляем локальный репозиторий, скачав изменения из удаленного репозитория (рис [-@fig:fig11]) 
![рисунок 11](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/11.png){ #fig:fig11 width=70% }
3.2. Переходим в каталог с шаблоном отчета по лабораторной работе №4 и проводим компиляцию шаблона с использованием Makefile.(рис [-@fig:fig12]) 
![рисунок 12](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/12.png){ #fig:fig12 width=70% }
3.3. Удаляем полученные файлы с использованием Makefile.(рис [-@fig:fig13])
![рисунок 13](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/13.png){ #fig:fig13 width=70% }
3.4.Проверяем, что после этой команды файлы report.pdf и report.docx были удалены (рис[-@fig:fig14]) 
![рисунок 14](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/14.png){ #fig:fig14 width=70% }
3.5.Открываем файл report.md c помощью любого текстового редактора, например gedit(рис [-@fig:fig15]) 
![рисунок 15](/home/smakopyan/work/study/2022-2023/Архитектура компьютера/arch-pc/labs/lab04/report/image/15.png){ #fig:fig15 width=70% }
3.6. Загружаем файлы на github
# Выводы
В результате данной лабораторной работы, я освоила процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

::: {#refs}
:::

