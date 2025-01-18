# Projekt zaliczeniowy
Praca_zaliczeniowa z kierunku ALK PYTHON DEV PD2

Do poprawnego działania projektu wymagane są następujące pakiety:
- import numpy as np
- import pandas as pd
- import glob
- import os
- import matplotlib.pyplot as plt
- import folium
- from folium.plugins import MarkerCluster

W poniższej linijce należy podać lokalizację folderu w którym znajduje się baza:
- os.chdir('C:/Users/micha/Jupyter projekty') #ustawienie folderu


# WNIOSKI:
Otrzymane dane wymagały wstępnej eksploracji w celu przygotowania zbioru do analizy. Analiza została przeprowadzona po usunięciu duplikatów, ujednoliceniu typów pojazdów i kategorii czynników wypadków.

Przed opisem wykonanej analizy koniecznym jest podkreślenie, że wyniki oraz wnioski są zależne od przyjętych założeń.
Do określenia najniebezpieczniejszych czynników wypadków w każdej dzielnicy Nowego Jorku zostało przyjęte założenie, że miarą najniebezpieczniejszych czynników wypadków jest liczba ofiar śmiertelnych. Do prezentacji opisanej statystyki został wykorzystany wykres kolumnowy skumulowany, dzięki któremu istnieje możliwość porównania na jednej grafice czynników mających wpływ na wystąpienie wypadków ze skutkiem śmiertelnym dla wszystkich dzielnic. Wartym rozważenia w dalszej eksploracji byłoby wyłączenie kategorii ‘Unspecified’ spośród czynników wypadków.

Liczba ofiar śmiertelnych i poszkodowanych z powodu szybkiej jazdy również została zaprezentowana na wykresie kolumnowym skumulowanym. W Brooklynie odnotowano najwyższą spośród wszystkich dzielnic liczbę poszkodowanych przekraczającą 1000 osób. Interesującym krokiem byłoby przedstawienie opisanej analizy z podziałem na lata, w których miało miejsce zdarzenie.
Przed wykonaniem selekcji 3 najczęstszych czynników wypadków z podziałem na dzielnice oraz ogółem dla całego miasta została wyłączona wspomniana wcześniej kategoria ‘Unspecified’. Najczęstszą przyczyną wypadków w każdej z dzielnic okazała się nieuwaga kierowcy.

W celu określenia jakie typy pojazdów uczestniczyły w wypadkach, zostały zliczone wystąpienia VEHICLE TYPE CODE 1 oraz VEHICLE TYPE CODE 2. Do wykonania zliczenia konieczne było ujednolicenie kategorii: ‘STATION WAGON/SPORT UTILITY VEHICLE’, które zostało zrealizowane na etapie przygotowania zbioru do analizy.

Najczęstsze miejsca wystąpienia wypadków zostały przedstawione z wykorzystaniem biblioteki folium. Baza danych prezentowana na mapie została zawężona do wypadków śmiertelnych, które miały miejsce w 2018 roku. 
Analizowany zbiór danych umożliwia przeprowadzenie kolejnych analiz, np.:
-	statystyka dotycząca godziny zdarzenia – w jakich godzinach wypadki statystycznie zdarzają się najczęściej;
-	statystyki dotyczące udziału pieszych i rowerzystów w wypadkach;
-	przedstawienie zdarzeń w ujęciu rocznym w podziale na poszczególne dzielnice i całe miasto.
