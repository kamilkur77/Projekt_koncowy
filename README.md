# Projekt_koncowy
Prognozowanie sprzedaży w Walmart 
Przygotowanie Danych:

Na początku zaimportowaliśmy potrzebne biblioteki i wczytaliśmy dane z plików CSV: train.csv, test.csv, stores.csv, i features.csv.
Przeprowadziliśmy analizę wstępną danych, w tym wyświetliliśmy pierwsze wiersze i sprawdziliśmy, czy występują brakujące wartości.
Łączenie Danych:

Po wczytaniu danych połączyliśmy dane treningowe z danymi cech z użyciem wspólnych kolumn Store i Date, przy użyciu metody pd.merge. To pozwoliło nam uwzględnić dodatkowe informacje o sklepach i cechach w zbiorze treningowym.
Przygotowanie danych treningowych:

Połączone dane treningowe zostały przetworzone w celu przygotowania ich do modelowania. Zostaliśmy z danymi zawierającymi cechy (np. temperatura, ceny paliw) oraz etykietami (tygodniowe sprzedaże).
Modelowanie:

Zastosowaliśmy dwa proste modele: Model Średniej oraz Model Regresji Liniowej.
Model Średniej prognozuje sprzedaż na podstawie średniej sprzedaży ze zbioru treningowego.
Model Regresji Liniowej próbuje przewidzieć sprzedaż, wykorzystując różne cechy, takie jak temperatura, ceny paliw, itp.
Ocena Modeli:

Oceniliśmy modele za pomocą dwóch metryk: Mean Squared Error (MSE) i R-squared (R^2).
MSE mierzy błąd prognoz modelu, a niższa wartość jest lepsza.
R-squared ocenia, jak dobrze model pasuje do danych, a wyższa wartość jest lepsza.
Wnioski:

Model Średniej miał bardzo niską precyzję, co jest zrozumiałe, ponieważ opiera się tylko na średnich wartościach.
Model Regresji Liniowej miał lepszą precyzję, ale nadal nie był wystarczająco dokładny, o czym świadczy wysokie MSE i niski R-squared.
Wskazaliśmy, że potrzebne są bardziej zaawansowane modele i dalsza praca nad inżynierią cech oraz eksploracyjną analizą danych.
Dalsze Kroki:

Dalsza praca powinna obejmować bardziej zaawansowane modele regresji, takie jak lasy losowe, regresja grzbietowa lub maszyny wektorów nośnych.
Możemy eksplorować dane bardziej szczegółowo, identyfikując wzorce czasowe i sezonowość.
Inżynieria cech może polegać na tworzeniu nowych zmiennych lub przekształcaniu istniejących w celu poprawienia modelu.
Dostosowanie hiperparametrów modelu może także poprawić jego wydajność.
Podsumowując, w analizie danych i modelowaniu sprzedaży konieczne jest ciągłe doskonalenie i dostosowywanie modeli, aby uzyskać bardziej precyzyjne prognozy, co ma kluczowe znaczenie w podejmowaniu efektywnych decyzji biznesowych.
