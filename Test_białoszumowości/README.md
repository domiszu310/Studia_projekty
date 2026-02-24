# Analiza białoszumowości i symulacje testów statystycznych w szeregach czasowych

## Cel projektu
Głównym celem projektu było zbadanie skuteczności metod weryfikacji hipotezy o białoszumowości szeregów czasowych. Analiza skupia się na porównaniu czułości podejścia graficznego oraz formalnych testów statystycznych w wykrywaniu zależności w danych.

## Zakres analizy
* **Implementacja testów**: Zautomatyzowanie testu graficznego opartego na regule trzech sigm oraz testów Boxa-Pierce'a i Ljungi-Boxa.
* **Badania symulacyjne**: Przeprowadzenie symulacji dla 7 typów szeregów o różnej charakterystyce (m.in. procesy i.i.d., błądzenie losowe, modele MA(1), trendy liniowe i sezonowe).
* **Wpływ parametrów**: Analiza zależności wyników od długości szeregu ($n$) oraz doboru maksymalnego opóźnienia ($h_{max}$).

## Technologie
* **Język**: R (R Markdown).
* **Kluczowe biblioteki**: `forecast`, `TSAFBook`, `dplyr`, `knitr`, `kableExtra`.

## Kluczowe wnioski
Symulacje wykazały, że **testy formalne są znacznie bardziej wrażliwe** na obecność autokorelacji niż metody graficzne, szczególnie w przypadku modeli ruchomej średniej (MA) oraz błądzenia losowego. Ponadto testy są najsurowsze dla dłuższych szeregów czasowych przy małych wartościach opóźnienia.
