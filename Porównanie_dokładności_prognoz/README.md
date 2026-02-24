# Prognozowanie szeregów czasowych - analiza porównawcza modeli (S)ARIMA, ETS i dekompozycji

## Cel projektu
Głównym celem analizy było porównanie skuteczności różnych metod prognozowania kwartalnego indeksu handlu detalicznego w strefie euro. Projekt bada, jak modele radzą sobie z silnym trendem, sezonowością oraz nagłymi zmianami strukturalnymi, takimi jak kryzys finansowy z 2008 roku.

## Wykorzystane metody
* **Modele (S)ARIMA**: Pełna procedura identyfikacji z uwzględnieniem transformacji Boxa-Coxa oraz różnicowania sezonowego.
* **Algorytmy wygładzania wykładniczego (ETS)**: Porównanie prostego wygładzania, algorytmu Holta oraz Holta-Wintersa (warianty addytywne i multiplikatywne).
* **Modele dekompozycji**: Regresja z trendem liniowym, kwadratowym i sześciennym oraz sezonowością.
* **Metoda referencyjna**: Sezonowa metoda naiwna (Seasonal Naive).

## Technologie i miary
* **Narzędzia**: Język R, biblioteki `forecast`, `fpp2`, `ggplot2`.
* **Miary dokładności**: Porównanie modeli na zbiorze testowym przy użyciu miar RMSE, MAE, MAPE oraz MASE.

## Wyniki i Wnioski
Model **SARIMA$(0, 1, 4)(0, 1, 0)_4$** okazał się bezkonkurencyjny, osiągając najniższe błędy prognoz i jako jedyny uzyskując wartość MASE < 1, co oznacza wyższą skuteczność od metody naiwnej. Ponadto pokazano, że modele ARIMA cechują się większą elastycznością w reagowaniu na gwałtowne zmiany trendu niż klasyczna dekompozycja.
