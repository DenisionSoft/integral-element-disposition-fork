# Fork of IntegralElementDisposition ETU project

## Overview

This repository contains a fork of the project practice project for the second year of Electrotechnical University.

My task was to develop an XML parser to read the XML file with the scheme and load in into the program for further processing, and then save the result back to the XML file.
Specifically, most of my work was done in the `Parser.cpp` file.

This project was written in C++ using Qt framework.

It was developed in collaboration with [Dmitry Trukhman](https://github.com/Qusild) and [Gleb Lyakh](https://github.com/WhoLeb).
The original licence referring to Gleb as 'WhoLeb' is included in the LICENSE file.

## Description

The original task as descibed in a README file of the parent repository (in Russian):

Учебная практика, второй курс.

Требуется разработать визуальный редактор, позволяющий оптимально (с точки зрения суммарной длины проводов) размещать интегральные микросхемы на двумерной однослойной плате. 
Плата представляет собой двумерную сетку, разбитую на одинаковые квадраты. Каждая интегральная схема может занимать 1 квадрат  и может быть связана с произвольным числом других интегральных схем. Таким образом, схема моделируется неориентированным графом, в котором вершинами являются схемы, а ребрами- соединения (между парой вершин может быть несколько ребер!).  Соединения на плате между схемами идут строго параллельно и перпендикулярно (по клеточкам) (см. Манхеттенское расстояние). Для оптимальной разводки платы требуется чтобы провода в каждой клеточке не пересекались (крест-на крест) и суммарная длина проводов на всю плату должна быть минимальна. 
   
Схема задаётся в виде XML-файла, в котором  указан размер платы (прямоугольник — число клеток по веритикале и горизонтали). Для каждой интегральной   схемы  в файле указывается расположение на плате и  список связей с другими интегральными схемами. Помимо этого в файле указывается  Структуру XML-файла студент / группа разрабатывает самостоятельно. Описание структуры XML-файла должно быть приведено в отчёте по практике.
Пользователю редактора должны быть доступны следующие функции:
<ul>
  <li>загрузка схемы;</li>
  <li>добавление в схему новых интегральных схем;</li>
  <li>возможность задания имени интегральной схемы и связей с другими интегральными схемами. Для каждой связи также должно задаваться имя;</li>
  <li>оптимизация размещения интегральных схем на плате по критерию минимальной суммарной длины проводов при отсутствии их пересечений.</li>
  <li>сохранение схемы в файл с возможностью его последующей загрузки в редактор.</li>
</ul>
