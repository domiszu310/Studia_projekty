# Odkrywanie ukrytych struktur i wizualizacja danych wielowymiarowych - analiza zbioru Titanic metodą MDS

## Cel projektu
Głównym celem analizy było zidentyfikowanie naturalnych skupisk pasażerów Titanica oraz ukrytych wzorców, które mogły mieć wpływ na ich ocalenie. Badanie przeprowadzono w sposób nienadzorowany (bez wstępnego użycia zmiennej o przeżyciu), aby sprawdzić, czy struktura danych sama w sobie odzwierciedla szanse na przetrwanie.

## Metodyka pracy
* **Przygotowanie danych**: Czyszczenie zbioru, konwersja typów zmiennych oraz obsługa brakujących wartości (imputacja metodą k-najbliższych sąsiadów - kNN dla zmiennej wieku).
* **Redukcja wymiarowości**: Zastosowanie metrycznego skalowania wielowymiarowego (MDS) w celu odwzorowania wielowymiarowej przestrzeni cech na płaszczyznę 2D przy zachowaniu oryginalnych odległości między obiektami.
* **Diagnostyka**: Ocena jakości odwzorowania przy użyciu kryterium STRESS oraz diagramu Sheparda.
* **Wizualizacja i interpretacja**: Analiza graficzna uzyskanych skupisk pod kątem płci, klasy pasażerskiej oraz wieku.

## Technologie
* **Język**: R (R Markdown).
* **Kluczowe biblioteki**: `ggplot2`, `cluster` (funkcja daisy), `MASS`, `VIM` (imputacja kNN), `DataExplorer`.

## Kluczowe wnioski
Wizualizacja MDS wyraźnie wyodrębniła skupiska pasażerów ze względu na płeć oraz klasę podróży, co potwierdziło silną zależność między strukturą danych a ocaleniem. Analiza wykazała, że największe szanse na przeżycie miały kobiety z pierwszej i drugiej klasy. Ponadto płeć i klasa miały kluczowy wpływ na przetrwanie, przewyższając znaczenie wieku.

## Uwagi techniczne
Ze względu na ograniczenia rozmiaru plików platformy GitHub raport został podzielony na dwie części:
  * **[Titanic_1.pdf](./Titanic_1.pdf)** – cel analizy oraz odpowiednie przygotowanie danych do dalszej analizy,
  * **[Titanic_2.pdf](./Titanic_2.pdf)** – redukcja wymiarowości (MDS) oraz diagram Sheparda wraz z komentarzem (ze względu na bardzo duży rozmiar, plik został skompresowany),
  * **[Titanic_3.pdf](./Titanic_3.pdf)** – wizualizacja wyników MDS wraz z komentarzem i wnioskami cząstkowymi.

Pełny, nieskompresowany raport można wygenerować, uruchamiając plik `Titanic.Rmd` np. w RStudio.

