# Projekt koncepcji prowadzenie wsparcia w oparciu o moduł CRM #

##Struktura

1. Kampania – główne działy firmy (Dział Produkcji, Dział Wsparcia, Dział Sprzedaży, Zarząd i wsparcie zarządu).
2. 	Projekty  - jako uszczegółowienie Kampanii 
•	Dział Produkcji i Dział wsparcia moduły: Księga, Kadry płace itp… (zgodne z azuredevops),
•	Dział sprzedaży: Marketing, Zespół Accantmenagerów, DWS.
•	Zarząd i wsparcie zarządu: Prezes, HR, Recepcja
3. Zadania - zgłoszenia serwisowe, inne zadania 
4. Zdarzenia - rejestracja telefonów


## Procesy

1. Procesy podstawowe:

W zakresie wsparcia partnerów:
Zdarzenie (incydent) ->znamy rozwianie- >Zamykamy zdarzenie

I. Telefon 

Nowe zdarzenie -> Wybieramy Pola na formularzu do uzupełnienia: Partner lub/i Klient (możliwosć wyszukania po licencji), Tytuł (Nazwa), Treść(Opis),Prowadzący (pracownik sonety), Przedstawiciel, liczkik,Stan zadania, 
Powinny wyświetlać się dodatkowe informacje o kliencie (np.Zakaz kontaktu)-> Po zakończonym zdarzeniu pytanie czy utworzyć zadania (wybieramy jeśli temat nie zakończony)->
Jeśli wybrano "Nie" zadrzenie zamykykane ze stanem Zakończony.


Nowe zdarzenie -> Wybieramy Pola na formularzu do uzupełnienia: Partner lub/i Klient (możliwosć wyszukania po licencji), Tytuł (Nazwa), Treść(Opis),Prowadzący (pracownik sonety), Przedstawiciel, liczkik,Stan zadania, 
Powinny wyświetlać się dodatkowe informacje o kliencie (np.Zakaz kontaktu)-> Po zakończonym zdarzeniu pytanie czy utworzyć zadania (wybieramy jeśli temat nie zakończony)->zamykamy zdarzenie tworzac zadanie po zatwierdzeniu "Tak" generowane jest nowe zadanie wybór definicji,
Otwiera się formularz zadania ->Uzupełniamy dodatkowe iformacje priorytet, stan zgłoszony.????

Zdarzenie ->nie znamy rozwiązania-> zamykamy zdarzenie tworzac zadanie-> Analiza (nowe zadanie) - > nie mamy rozwiązania -> Przekazanie na produkcje  (Aure Devops) - > zwrotna informacja o zakończonym zadaniu.

2.Procesy Dodatkowe

Zadanie (nowe zadanie zlecone przez inny dział) - > Analiza / realizacja-> Zamykamy zadanie
Zadanie (nowe zadanie zlecone przez inny dział) - > Analiza -> nie znamy rozwiązania -> Przekazanie na produkcje  (Aure Devops) - > zwrotna informacja o zakończonym zadaniu.
 
Do analizy skrócenie procesu, druga linia wsparcia określenie osoby z dzialu produkcji !!!!

## Mapowanie do istniejących pól

1.Zadanie - zgłoszenie serwisowe

* Tytuł - Nazwa (Zadanie)

* Treść zgłoszenia - Opis (Zadanie)
* Prowadzący pracownik Sonety - Prowadzący (Zadanie)
* Osoba kontaktowa - Przedstawiciel (Zadanie)
* Partner - Do dodania
* Klient - Do dodania
* Stan  - Satan(Zadania)
Zgłoszony – Partner zgłosił ale jeszcze nikt nie przeanalizował 
Analizowany – Konsultant analizuje temat 
W realizacji – przyjęto do realizacji, np. poprawiamy błąd w produkcji 
Zakończony – temat zrealizowany produkcyjnie/udzielono wsparcia  
Lub informacja o tym że temat został odrzucony nie będziemy realizować 
Anulowany- partner sam anulował zgłoszenie 
* Typ (bład,  nowa funkcja programistyczne reklamacja) - Do dodania
* Nie może to być defnicja bo jest niezmienna!
* Numer wersji - Do dodania
* Tryb zgłoszenia - Definicja zgłoszenia (Zadania)
* Interfejs - Do dodania
* Moduł - Do dodania - zgodny z azuredevops i cennikiem
* Obaszar - Do dodania
* Data zgłoszenia - Rozpoczęcie (Zadania)
* Data zakończenia - Zakończenie (Zadania)
* Stoper (Zadania)
* Nazwa produktu (enova365 oraz Triva)
* Notataka - Uwagi (Zadania)
* Załaczniki - Asystent(Zadanie)
* Priorytet (Krytyczny/Wysoki/Normalny/Niski) - Pryiorytet (Zadania)
* Informacja o kliencie/partnarze - Do dodania pobierać z kartoteki kontrahenta Uwagi handlowe?

* Słowa kluczowe - pole słownikowe -  Do dodania -  pole które pozwoli nam wyszukiwać rozwiazania z załatwionych 
* Baza wiedzy - linki Do dodania
* Informacja o licencji

1.Zdarzenie (incydent) - zgłoszenie telefoniczne 

* Tytuł - Nazwa (Zdarzenie)
* Treść zgłoszenia - Opis (Zdarzenie)
* Prowadzący pracownik Sonety - Prowadzący (Zdarzenie)
* Osoba kontaktowa - Przedstawiciel (Zdarzenie)
* Partner - Do dodania
* Klient - Do dodania
* Stan (rózny dla definicji) - Stan (Zdarzenie)
* Typ (bład,  nowa funkcja programistyczne reklamacja) - Do dodania
* Nie może to być defnicja bo jest niezmienna!
* Numer wersji - Do dodania
* Tryb zgłoszenia - Definicja zgłoszenia (Zdarzenia)
* Interfejs - Do dodania
* Moduł - Do dodania - zgodny z azuredevops i cennikiem
* Obaszar - Do dodania
* Data zgłoszenia - Rozpoczęcie (Zadania)
* Data zakończenia - Zakończenie (Zadania)
* Stoper (Zadania)
* Nazwa produktu (enova365 oraz Triva)
* Notataka - Uwagi (Zadania)
* Załaczniki - Asystent(Zadanie)
* Informacja o kliencie/partnarze - Do dodania pobierać z kartoteki kontrahenta Uwagi handlowe?


* Słowa kluczowe - pole słownikowe -  Do dodania -  pole które pozwoli nam wyszukiwać rozwiazania z załatwionych 
* Baza wiedzy - linki Do dodania
* Informacja o licencji


## Konfiguracja

1. Defincije zadań 

* Zgłoszenie Serwisowe -ZS/Rok/kolejny Numer

Stan  - Stan(Zadania)
   Zgłoszony – Partner zgłosił ale jeszcze nikt nie przeanalizował 
   Analizowany – Konsultant analizuje temat 
   W realizacji – przyjęto do realizacji, np. poprawiamy błąd w produkcji 
   Zakończony – temat zrealizowany produkcyjnie/udzielono wsparcia  
   Lub informacja o tym że temat został odrzucony nie będziemy realizować 
   Anulowany- partner sam anulował zgłoszenie 

* Zgłoszenie Wewnętrzne - ZW/Rok/lolejny numer

Stan: 
  Zgłoszony  
  W realizacji
  Zakończony 
  Anulowany

* Komunikat - KOM/rok/kolejny numer (zastępuje globalne zgłoszenie)
Szkolenie - SZ/rok/kolejny numer (szkolenie prezentacja)

Stan: 
  Zgłoszony  
  W realizacji
  Zakończony 
  Anulowany

2. Definicje zdarzeń

Zgłoszenie telefoniczne 

ZT/Rok/kolejny numer
Stan: 
  W realizacji
  Zakończony 



3. Formularz użytkownika

4.integracja

zmiana stanu eksportuje do AzureDevops

5. Komunikacja z działęm spzredaży- informacja z cechy zakas kontaktu
Dodatkowe komunikaty o partnerze kliencie do ustalenia z działem sprzedaży.

