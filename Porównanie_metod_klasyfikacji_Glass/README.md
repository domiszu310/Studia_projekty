# Porównanie dokładności klasycznych i zaawansowanych metod klasyfikacji - analiza skuteczności modeli na zbiorze danych Glass

## Cel projektu
Celem analizy było porównanie dokładności szerokiej gamy algorytmów klasyfikacji w celu wyłonienia optymalnego modelu dla zbioru danych `Glass`. Projekt bada, czy zaawansowane metody klasyfikacji oraz specyficzne schematy walidacji istotnie poprawiają wyniki względem metod klasycznych.

## Wykorzystane algorytmy i techniki
Projekt został podzielony na dwie główne grupy metod:

1. **Klasyczne metody klasyfikacji:**
   * k-najbliższych sąsiadów (**kNN**) – z optymalizacją parametru $k$.
   * **Drzewa klasyfikacji** – z optymalizacją parametrów `cp`, `minsplit` oraz `maxdepth`.
   * **Naiwny Klasyfikator Bayesowski** – porównanie modeli parametrycznych i nieparametrycznych.

2. **Zaawansowane metody klasyfikacji:**
   * Metoda wektorów nośnych (**SVM**) – optymalizacja jąder (gaussowskie, liniowe) oraz parametrów `cost` i `gamma`.
   * **Rodziny klasyfikatorów**: Bagging, Boosting (AdaBoost) oraz Random Forest.

3. **Walidacja i ocena dokładności:**
   * Wykorzystanie zaawansowanych schematów oceny błędu: **10-krotna walidacja krzyżowa** oraz **Bootstrap** i **Bootstrap 632plus**.
   * Analiza ważności cech i macierzy pomyłek.

## Technologie
* **Język**: R (R Markdown).
* **Kluczowe biblioteki**: `randomForest`, `e1071` (SVM), `adabag`, `ipred` (Bagging), `rpart`, `klaR`, `ggplot2`.

## Kluczowe wnioski
Najlepsze wyniki klasyfikacji uzyskały metody oparte na drzewach - **Random Forest** oraz **Bagging** - z wykorzystaniem schematu **Bootstrap 632plus**, co pozwoliło na skuteczne uniknięcie przeuczenia modelu. Analiza wykazała, że cechy takie jak zawartość glinu (Al) i magnezu (Mg) mają najwyższą zdolność dyskryminacyjną w badanym zbiorze.
