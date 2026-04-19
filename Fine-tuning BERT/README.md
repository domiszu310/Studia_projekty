# Optymalizacja modeli BERT i LSTM – Analiza Kompromisu

Ten projekt stanowi mój indywidualny wkład analityczny w ramach szerszego projektu grupowego dotyczącego fine-tuningu modelu BERT oraz jego porównania z modelem LSTM. Repozytorium zawiera raporty z badań nad wyborem optymalnych modeli z uwzględnieniem kompromisu między dokładnością a zużyciem zasobów obliczeniowych.

## Cel analizy
Głównym celem mojej części projektu było znalezienie "złotego środka" dla procesu fine-tuningu. Badałam, jak zamrażanie warstw oraz LR wpływa na jakość generalizacji i koszty obliczeniowe. 

W tym repozytorium odpowiadam na pytania:
* Jak parametr Learning Rate oraz liczba zamrożonych warstw wpływają na dokładność uczenia w modelu **BERT**?
* Jakie jest rzeczywiste zużycie zasobów (VRAM GPU, RAM, czas treningu) dla poszczególnych konfiguracji?
* Jaka jest optymalna liczba epok dla modelu **LSTM**, aby uniknąć przeuczenia?

## Technologie
* **Środowisko:** Google Colab
* **Analiza i Wizualizacja Danych:** R w ipyhn (ggplot2, dplyr, tidyr)

## Struktura repozytorium
* `analiza_kompromisu_BERT.ipynb` - analizę kosztów vs jakości na różnego rodzaju wykresach m.in. wykresach rozrzutu.
* `analiza_epok_LSTM.ipynb` - wykresy i wnioski dotyczące doboru optymalnej liczby epok dla sieci LSTM.

---
*Projekt zrealizowany w ramach pracy grupowej. Ze względu na przejrzystość, to repozytorium zawiera wyłącznie pliki odpowiadające za moją część analityczną i wizualizacyjną.*
