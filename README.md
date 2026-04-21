# Analiza odejść klientów - Telco-Customer-Churn

## Autorzy:
* Zuzanna Jastrzębska
* Kacper Józefkowicz

## Opis projektu
Projekt ten przedstawia kompleksową analizę opisową zachowań klientów firmy telekomunikacyjnej. Projekt jest częścią przedmiotu Eksploracja Danych w roku akademickim 25/26.

## Zbiór danych
Analiza opiera się na zbiorze danych `WA_Fn-UseC_-Telco-Customer-Churn.csv`.
* **Źródło:** [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
* **Zawartość:** Dane demograficzne, informacje o posiadanych usługach, stażu klienta oraz opłatach.

## Wykorzystane technologie
* **Język:** R
* **Formaty plików:** RMarkdown (`.Rmd`) wykorzystany do wygenerowania końcowego sprawozdania w formacie PDF.

## Struktura i etapy analizy

Projekt został podzielony na cztery główne etapy analityczne:

### Etap 1: Przygotowanie danych
* Wczytanie zbioru danych i prawidłowe mapowanie typów zmiennych (zmienne jakościowe jako `factor`, ilościowe jako `numeric`).
* Czyszczenie danych, w tym usunięcie unikalnych identyfikatorów niemających znaczenia analitycznego (ID klienta).
* Identyfikacja braków danych oraz nietypowych wartości.

### Etap 2: Analiza opisowa
* Wyznaczenie podstawowych wskaźników sumarycznych (miary położenia i rozproszenia) dla poszczególnych zmiennych.
* Zobrazowanie rozkładów cech za pomocą odpowiednich wykresów (wykresy słupkowe, wykresy pudełkowe).
* Badanie zależności między zmiennymi ciągłymi z wykorzystaniem wykresów rozrzutu.

### Etap 3: Analiza z podziałem na grupy (Churn)
* Szczegółowe porównanie profili klientów podzielonych na dwie grupy docelowe:
    * **Grupa 1:** Klienci, którzy odeszli (`Churn == 'Yes'`).
    * **Grupa 2:** Lojalni klienci, pozostający w firmie (`Churn == 'No'`).
* Wskazanie cech charakteryzujących się największym zróżnicowaniem pomiędzy obiema grupami.

### Etap 4: Podsumowanie i rekomendacje biznesowe
* Wnioski podsumowujące główne cechy klientów oraz ich preferencje usługowe.
* Identyfikacja kluczowych przyczyn zjawiska odchodzenia klientów.
* Zestaw propozycji działań zaradczych dla firmy telekomunikacyjnej, które mogą skutecznie przeciwdziałać rezygnacjom.

## Jak uruchomić projekt?
1. Sklonuj repozytorium na swój dysk lokalny.
2. Upewnij się, że plik z danymi `WA_Fn-UseC_-Telco-Customer-Churn.csv` znajduje się w katalogu roboczym.
3. Otwórz plik `.Rmd` w środowisku np. RStudio lub plik `.pdf` do bezpośredniego podglądu wygenerowanego raportu.
