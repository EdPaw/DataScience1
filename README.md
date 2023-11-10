# DataScience1
10.11.2023 Zadanie z kursu CODE:ME

POBRANIE DANYCH
<br />1. Pobrano dane GUS Bank Danych Lokalnych w formacie .xlsx
<br />2. Wybrano następujące dane: 

Kategoria:	K4	RYNEK PRACY 
Grupa:	G479	PRACUJĄCY, ZATRUDNIENI I PRZECIĘTNE ZATRUDNIENIE WEDŁUG PKD
Podgrupa:	P2988	Zatrudnieni wg sekcji, sektorów własności i płci   
Wymiary: Sektory własności; Płeć; Sekcje wg PKD 2007; Lata

Wybrano: Rok 2021, Sektowy własności: All, Płeć: All, Sekcje wg PKD 2007: All

<br />3. Utworzono dane słownikowe dla sekcji w formacie .xlsx (ręcznie)

TRANSFORMACJE
<br />4. Sprawdzono czy są nulle i duplikaty (brak)
<br />5. Dołączono słownik dla sekcji funkcją merge
<br />7. Usunięto wszystkie wiersze, gdzie w komórce mogła występować wartość 'ogółem'
<br />9. Pozostawiono tylko dane dla 'Nazwa' = 'POLSKA' (zrezygnowano z podziału na województwa)
<br />11. Usunięto zbędne kolumny (nieprzydatne pod kątem analitycznym)
<br />13. Zmieniono typy danych object na str
<br />15. Sortowanie po 'Wartosc', 5 pierwszych, 5 ostatnich

WYKRES
<br />11. Utworzono bar chart horyzontalny 'Zatrudnieni wg sekcji - 2021', zmodyfikowano tytuł, podpisy osi, labele

ZAPIS DO BAZY
<br />12. Tworzenie bazy danych sqlite3
<br />13. Tworzenie i zapis dataframe do tabeli
<br />15. Pokazanie tabeli
<br />17. Zamknięcie bazy

BIBLIOTEKI
<br />sqlite3
<br />matplotlib.pyplot
<br />google.colab import drive
<br />pandas
