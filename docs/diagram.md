'''mermaid
graph TD
    %% Węzeł początkowy
    Start((START)) --> Menu[Menu Głowne - Aplikacja Budżetowa Euruś]

        %% Ścieżka 1: Dodawanie wydatku
        Menu --> Option1[1.Dodaj Wydatek]
        Option1 --> InputData[/Wprowadz dane: Kwota, Kategoria, Data]
        Input Data --> Added[Dodano do listy]

        %% Ścieżka 2: Raport
        Menu --> Option2[2. Generuj raport]
        Option2 --> SelectPeriod[/Wybierz Okres/]
        SelectPeriod --> Calc[Obliczanie Podsumowania Wydatków]

        %% Ścieżka 3: Zapis
        Menu --> Option3[3. Zapisz Dane]
        Option3 --> Export[Export to .txt]
        Export --> Saved[Dane zapisane wpliku .txt]

        %% Ścieżka 4: Wyjście
        Menu --> Option4[4. Wyjście]
        Option4 --> Stop ((Koniec))