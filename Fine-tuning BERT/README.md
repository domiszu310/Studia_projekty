# Analiza Kompromisu - optymalizacja modeli BERT

Ten projekt stanowi mój indywidualny wkład analityczny w ramach szerszego projektu grupowego dotyczącego fine-tuningu modelu BERT. Repozytorium zawiera raport z badań nad wyborem optymalnych modeli z uwzględnieniem kompromisu między dokładnością a zużyciem zasobów obliczeniowych.

## Cel analizy
Głównym celem mojej części projektu było znalezienie "złotego środka" dla procesu fine-tuningu. Badałam, jak zamrażanie warstw oraz LR wpływa na jakość generalizacji i koszty obliczeniowe. 

W tym repozytorium odpowiadam na pytania:
* Jak parametr Learning Rate oraz liczba zamrożonych warstw wpływają na dokładność uczenia w modelu **BERT**?
* Jakie jest rzeczywiste zużycie zasobów (VRAM GPU, RAM, czas treningu) dla poszczególnych konfiguracji?

## Technologie
* **Środowisko:** Google Colab, Jupiter Notebook
* **Analiza i Wizualizacja Danych:** R (ggplot2, dplyr, tidyr)

## Struktura repozytorium
* `Opisy baz danych.docx` - charakterystyka baz danych wykorzystanych w projekcie.
* `Analiza kompromisu.ipynb` - analizę kosztów vs jakości na różnego rodzaju wykresach m.in. wykresach rozrzutu.

---
*Projekt zrealizowany w ramach pracy grupowej. Ze względu na przejrzystość, to repozytorium zawiera wyłącznie pliki odpowiadające za moją część analityczną i wizualizacyjną.*
