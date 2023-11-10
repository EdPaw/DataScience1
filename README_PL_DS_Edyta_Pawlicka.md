# Data Science CODE:ME Homework 1 Edyta Pawlicka
10.11.2023 Zadanie z kursu CODE:ME

1. Pobrano dane GUS Bank Danych Lokalnych w formacie .xlsx
2. Wybrano następujące dane: 

Kategoria:	K4	RYNEK PRACY 
Grupa:	G479	PRACUJĄCY, ZATRUDNIENI I PRZECIĘTNE ZATRUDNIENIE WEDŁUG PKD
Podgrupa:	P2988	Zatrudnieni wg sekcji, sektorów własności i płci   
Wymiary: Sektory własności; Płeć; Sekcje wg PKD 2007; Lata

Wybrano: Rok 2021, Sektowy własności: All, Płeć: All, Sekcje wg PKD 2007: All

3. Utworzono dane słownikowe dla sekcji w formacie .xlsx (ręcznie)

TRANSFORMACJE
4. Sprawdzono czy są nulle i duplikaty (brak)
5. Dołączono słownik dla sekcji funkcją merge
6. Usunięto wszystkie wiersze, gdzie w komórce mogła występować wartość 'ogółem'
7. Pozostawiono tylko dane dla 'Nazwa' = 'POLSKA' (zrezygnowano z podziału na województwa)
8. Usunięto zbędne kolumny (nieprzydatne pod kątem analitycznym)
9. Zmieniono typy danych object na str
10. Sortowanie po 'Wartosc', 5 pierwszych, 5 ostatnich

WYKRES
11. Utworzono bar chart horyzontalny 'Zatrudnieni wg sekcji - 2021', zmodyfikowano tytuł, podpisy osi, labele

ZAPIS DO BAZY
12. Tworzenie bazy danych sqlite3
13. Tworzenie i zapis dataframe do tabeli
14. Pokazanie tabeli
15. Zamknięcie bazy

WYKORZYSTANE BIBLIOTEKI
sqlite3
matplotlib.pyplot
google.colab import drive
pandas
